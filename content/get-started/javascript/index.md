---
layout: docs
title: Javascript
seo_title: Bootstrap Components with TypeScript
description: Bootstrap JS components implemented with TypeScript. Learn about each plugin, our data and programmatic API options, and more.
toc: true
menu:
  get-started:
icon: fa-brands fa-js
weight: 31
---

{{< callout warning >}}
**Recommend using the Bootstrap official JS library**.
{{</ callout >}}

`fastbootstrap.js` is depend on [bootstrap.native](https://github.com/thednp/bootstrap.native) since 2.1, which is the Bootstrap JS components implemented in Typescript, but **does not support all options setting of Bootstrap components**.

{{< bs-table >}}
| Features | bootstrap.js | bootstrap.bundle.js |
| --- | --- | --- | --- |
| Minified  | ~ 60Kb | ~ 80Kb |
| Popper JS | - | popperjs/core |
| ES module | <i class="fa-solid fa-check icon-body"></i> | <i class="fa-solid fa-check icon-body"></i> |
{{</ bs-table >}}

{{< bs-table >}}
| JS | CDN |
| --- | --- |
| Bootstrap bundle | {{< param "bootstrap.cdn.js_bundle" >}} | 
{{</ bs-table >}}

## Data attributes 

Nearly all Bootstrap plugins can be enabled and configured through HTML alone with data attributes (our preferred way of using JavaScript functionality). Be sure to **only use one set of data attributes on a single element** (e.g., you cannot trigger a tooltip and modal from the same button.)

As options can be passed via data attributes or JavaScript, you can append an option name to `data-bs-`, as in `data-bs-animation="{value}"`. Make sure to change the case type of the option name from “camelCase” to “kebab-case” when passing the options via data attributes. For example, use `data-bs-custom-class="beautifier"` instead of `data-bs-customClass="beautifier"`.

As of Bootstrap 5.2.0, all components support an experimental reserved data attribute data-bs-config that can house simple component configuration as a JSON string. When an element has `data-bs-config='{"delay":0, "title":123}'` and `data-bs-title="456"` attributes, the final `title` value will be `456` and the separate data attributes will override values given on data-bs-config. In addition, existing data attributes are able to house JSON values like `data-bs-delay='{"show":0,"hide":150}'`.

The final configuration object is the merged result of `data-bs-config`, `data-bs-`, and `js object` where the latest given key-value overrides the others.

## Selectors 

We use the native `querySelector` and `querySelectorAll` methods to query DOM elements for performance reasons, so you must use valid selectors. If you use special selectors like `collapse:Example`, be sure to escape them.

## Events 

Bootstrap provides custom events for most plugins’ unique actions. Generally, these come in an infinitive and past participle form - where the infinitive (ex. `show`) is triggered at the start of an event, and its past participle form (ex. `shown`) is triggered on the completion of an action.

All infinitive events provide [preventDefault()](https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault) functionality. This provides the ability to stop the execution of an action before it starts. Returning false from an event handler will also automatically call `preventDefault()`.

```js
const myModal = document.querySelector('#myModal')

myModal.addEventListener('show.bs.modal', event => {
  return event.preventDefault() // stops modal from being shown
})
```

## Programmatic API 

All constructors accept an optional options object or nothing (which initiates a plugin with its default behavior):

```js
const myModalEl = document.querySelector('#myModal')
const modal = new bootstrap.Modal(myModalEl) // initialized with defaults

const configObject = { keyboard: false }
const modal1 = new bootstrap.Modal(myModalEl, configObject) // initialized with no keyboard
```

If you’d like to get a particular plugin instance, each plugin exposes a getInstance method. For example, to retrieve an instance directly from an element:

```js
bootstrap.Popover.getInstance(myPopoverEl)
```

This method will return `null` if an instance is not initiated over the requested element.

Alternatively, `getOrCreateInstance` can be used to get the instance associated with a DOM element, or create a new one in case it wasn’t initialized.

```js
bootstrap.Popover.getOrCreateInstance(myPopoverEl, configObject)
```

In case an instance wasn’t initialized, it may accept and use an optional configuration object as second argument.

### CSS selectors in constructors

In addition to the `getInstance` and `getOrCreateInstance` methods, all plugin constructors can accept a DOM element or a valid CSS selector as the first argument. Plugin elements are found with the `querySelector` method since our plugins only support a single element.

```js
const modal = new bootstrap.Modal('#myModal')
const dropdown = new bootstrap.Dropdown('[data-bs-toggle="dropdown"]')
const offcanvas = bootstrap.Offcanvas.getInstance('#myOffcanvas')
const alert = bootstrap.Alert.getOrCreateInstance('#myAlert')
```

### Asynchronous functions and transitions 

All programmatic API methods are **asynchronous** and return to the caller once the transition is started, but **before it ends**. In order to execute an action once the transition is complete, you can listen to the corresponding event.

```js
const myCollapseEl = document.querySelector('#myCollapse')

myCollapseEl.addEventListener('shown.bs.collapse', event => {
  // Action to execute once the collapsible area is expanded
})
```

In addition, a method call on a **transitioning component will be ignored**.

```js
const myCarouselEl = document.querySelector('#myCarousel')
const carousel = bootstrap.Carousel.getInstance(myCarouselEl) // Retrieve a Carousel instance

myCarouselEl.addEventListener('slid.bs.carousel', event => {
  carousel.to('2') // Will slide to the slide 2 as soon as the transition to slide 1 is finished
})

carousel.to('1') // Will start sliding to the slide 1 and returns to the caller
carousel.to('2') // !! Will be ignored, as the transition to the slide 1 is not finished !!
```

### "dispose" method 

While it may seem correct to use the `dispose` method immediately after `hide()`, it will lead to incorrect results. Here’s an example of the problem use:

```js
const myModal = document.querySelector('#myModal')
myModal.hide() // it is asynchronous

myModal.addEventListener('shown.bs.hidden', event => {
  myModal.dispose()
})
```

### Default settings 

You can change the default settings for a plugin by modifying the plugin’s `Constructor.Default` object:

```js
// changes default for the modal plugin's `keyboard` option to false
bootstrap.Modal.Default.keyboard = false
```

## Methods and properties

Every Bootstrap plugin exposes the following methods and static properties.

{{< bs-table >}}
| Method | Description |
| --- | --- |
| `dispose` | Destroys an element’s modal. (Removes stored data on the DOM element) |
| `getInstance` | *Static* method which allows you to get the modal instance associated with a DOM element. |
| `getOrCreateInstance` | *Static* method which allows you to get the modal instance associated with a DOM element, or create a new one in case it wasn’t initialized. |
{{</ bs-table >}}


## Disabled JavaScript 

Bootstrap’s plugins have no special fallback when JavaScript is disabled. If you care about the user experience in this case, use `<noscript>` to explain the situation (and how to re-enable JavaScript) to your users, and/or add your own custom fallbacks.