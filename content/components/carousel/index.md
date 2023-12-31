---
layout: docs
title: Carousel
description: "Carousel are slideshow for cycling through multiple elements such as images, videos, or text."
toc: true
tabs: true
group: surfaces
menu:
  components:
---

{{< tabs "carousel" >}}
{{< tab "Overview" >}}

**Bootstrap 5 Carousel component**

Responsive carousel built with the latest Bootstrap 5. Carousel is a slideshow cycling through different elements such as photos, videos, or text. Many examples and easy tutorials.

## Carousel example

Carousel allows navigate the multiple images and displaing in sequence in the same place.

{{< example class="bd-example-carousel" >}}
<div id="carouselBasicExample" class="carousel slide" data-bs-ride="true">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselBasicExample" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselBasicExample" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselBasicExample" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="/images/carousel/1.jpg" class="d-block w-100" alt="frog" />
    </div>
    <div class="carousel-item">
      <img src="/images/carousel/2.jpg" class="d-block w-100" alt="frog" />
    </div>
    <div class="carousel-item">
      <img src="/images/carousel/3.jpg" class="d-block w-100" alt="frog" />
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselBasicExample" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselBasicExample" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
{{</ example >}}

## How it works

The carousel is a slideshow for cycling through a series of content, built with CSS 3D transforms and a bit of JavaScript. It works with a series of images, text, or custom markup. It also includes support for previous/next controls and indicators.

In browsers where the [Page Visibility API](https://www.w3.org/TR/page-visibility/) is supported, the carousel will avoid sliding when the webpage is not visible to the user (such as when the browser tab is inactive, the browser window is minimized, etc.).

{{< callout info >}}
The animation effect of this component is dependent on the prefers-reduced-motion media query. See the [reduced motion section of our accessibility](https://getbootstrap.com/docs/5.2/getting-started/accessibility/#reduced-motion) documentation.
{{< /callout >}}

Please be aware that nested carousels are not supported, and carousels are generally not compliant with accessibility standards.

## Variations

Carousels don't automatically normalize slide dimensions. As such, you may need to use additional utilities or custom styles to appropriately size content. While carousels support previous/next controls and indicators, they're not explicitly required. Add and customize as you see fit.

**The `.active` class needs to be added to one of the slides** otherwise the carousel will not be visible. Also be sure to set a unique `id` on the `.carousel` for optional controls, especially if you're using multiple carousels on a single page. Control and indicator elements must have a `data-bs-target` attribute (or `href` for links) that matches the `id` of the `.carousel` element.

### Slides only

Here's a carousel with slides only. Note the presence of the `.d-block` and `.w-100` on carousel images to prevent browser default image alignment.

{{< example class="bd-example-carousel" >}}
<div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="/images/carousel/4.jpg" alt="Tokyo" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/5.jpg" alt="Shanghai" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/6.jpg" alt="Newyork" />
    </div>
  </div>
</div>
{{< /example >}}

### With controls

Adding in the previous and next controls. We recommend using `<button>` elements, but you can also use `<a>` elements with `role="button"`.

{{< example class="bd-example-carousel" >}}
<div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="/images/carousel/1.jpg" alt="frog" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/2.jpg" alt="frog" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/3.jpg" alt="frog" />
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
{{< /example >}}

### With indicators

You can also add the indicators to the carousel, alongside the controls, too.

{{< example class="bd-example-carousel" >}}
<div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="true">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="/images/carousel/1.jpg" alt="frog" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/2.jpg" alt="frog" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/3.jpg" alt="frog" />
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
{{< /example >}}

### With captions

Add captions to your slides easily with the `.carousel-caption` element within any `.carousel-item`. They can be easily hidden on smaller viewports, as shown below, with optional [display utilities]({{< docsref "display" >}}). We hide them initially with `.d-none` and bring them back on medium-sized devices with `.d-md-block`.

{{< example class="bd-example-carousel" >}}
<div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="false">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="/images/carousel/4.jpg" alt="Tokyo" />
      <div class="carousel-caption d-none d-md-block">
        <h5>Tokyo (Japan)</h5>
        <p>Some representative placeholder content for the first slide.</p>
      </div>
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/5.jpg" alt="Shanghai" />
      <div class="carousel-caption d-none d-md-block">
        <h5>Shanghai (China)</h5>
        <p>Some representative placeholder content for the second slide.</p>
      </div>
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/6.jpg" alt="Newyork" />
      <div class="carousel-caption d-none d-md-block">
        <h5>Newyork (United states)</h5>
        <p>Some representative placeholder content for the third slide.</p>
      </div>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
{{< /example >}}

### Crossfade

Add `.carousel-fade` to your carousel to animate slides with a fade transition instead of a slide. Depending on your carousel content (e.g., text only slides), you may want to add `.bg-body` or some custom CSS to the `.carousel-item`s for proper crossfading.

{{< example class="bd-example-carousel" >}}
<div id="carouselExampleFade" class="carousel slide carousel-fade" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="/images/carousel/1.jpg" alt="frog" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/2.jpg" alt="frog" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/3.jpg" alt="frog" />
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleFade" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleFade" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
{{< /example >}}

### Individual `.carousel-item` interval

Add `data-bs-interval=""` to a `.carousel-item` to change the amount of time to delay between automatically cycling to the next item.

{{< example class="bd-example-carousel" >}}
<div id="carouselExampleInterval" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active" data-bs-interval="10000">
      <img class="d-block w-100" src="/images/carousel/1.jpg" alt="frog" />
    </div>
    <div class="carousel-item" data-bs-interval="2000">
      <img class="d-block w-100" src="/images/carousel/2.jpg" alt="frog" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/3.jpg" alt="frog" />
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
{{< /example >}}

### Disable touch swiping

Carousels support swiping left/right on touchscreen devices to move between slides. This can be disabled using the `data-bs-touch` attribute. The example below also does not include the `data-bs-ride` attribute so it doesn't autoplay.

{{< example class="bd-example-carousel" >}}
<div id="carouselExampleControlsNoTouching" class="carousel slide" data-bs-touch="false">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="/images/carousel/4.jpg" alt="tokyo" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/5.jpg" alt="shanghai" />
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="/images/carousel/6.jpg" alt="newyork" />
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControlsNoTouching" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControlsNoTouching" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
{{< /example >}}

## Custom transition 

The transition duration of `.carousel-item` can be changed with the `$carousel-transition-duration` Sass variable before compiling or custom styles if you’re using the compiled CSS. If multiple transitions are applied, make sure the transform transition is defined first (eg. `transition: transform 2s ease, opacity .5s ease-out`).

{{</ tab >}}
{{< tab "API" >}}

## Usage

### Via data attributes

Use data attributes to easily control the position of the carousel. `data-bs-slide` accepts the keywords `prev` or `next`, which alters the slide position relative to its current position. Alternatively, use `data-bs-slide-to` to pass a raw slide index to the carousel `data-bs-slide-to="2"`, which shifts the slide position to a particular index beginning with `0`.

The `data-bs-ride="carousel"` attribute is used to mark a carousel as animating starting at page load. If you don't use `data-bs-ride="carousel"` to initialize your carousel, you have to initialize it yourself. **It cannot be used in combination with (redundant and unnecessary) explicit JavaScript initialization of the same carousel.**

### Via JavaScript

Call carousel manually with:

```js
const carousel = new bootstrap.Carousel('#myCarousel')
```

## Options

{{< markdown >}}
{{< partial "js-data-attributes.md" >}}
{{< /markdown >}}

{{< bs-table >}}
| Name | Type | Default | Description |
| --- | --- | --- | --- |
| `interval` | number | `5000` | The amount of time to delay between automatically cycling an item. |
| `keyboard` | boolean | `true` | Whether the carousel should react to keyboard events. |
| `pause` | string, boolean | `"hover"` | If set to `"hover"`, pauses the cycling of the carousel on `mouseenter` and resumes the cycling of the carousel on `mouseleave`. If set to `false`, hovering over the carousel won't pause it. On touch-enabled devices, when set to `"hover"`, cycling will pause on `touchend` (once the user finished interacting with the carousel) for two intervals, before automatically resuming. This is in addition to the mouse behavior. |
| `ride` | string, boolean | `false` | If set to `true`, autoplays the carousel after the user manually cycles the first item. If set to `"carousel"`, autoplays the carousel on load. |
| `touch` | boolean | `true` | Whether the carousel should support left/right swipe interactions on touchscreen devices. |
| `wrap` | boolean | `true` | Whether the carousel should cycle continuously or have hard stops. |
| `indicator` | string | `.carousel-indicators` | Specified the carousel indicator of the carousel. <span class="lozenge lozenge-new">NEW</span> |
{{< /bs-table >}}

## Methods

{{< callout danger >}}
{{< partial "callout-danger-async-methods.md" >}}
{{< /callout >}}

You can create a carousel instance with the carousel constructor, for example, to initialize with additional options and start cycling through items:

```js
const myCarouselElement = document.querySelector('#myCarousel')
const carousel = new bootstrap.Carousel(myCarouselElement, {
  interval: 2000,
  wrap: false
})
```

{{< bs-table >}}
| Method | Description |
| --- | --- |
| `cycle` | Cycles through the carousel items from left to right. |
| `dispose` | Destroys an element's carousel. (Removes stored data on the DOM element) |
| `getInstance` | Static method which allows you to get the carousel instance associated to a DOM element, you can use it like this: `bootstrap.Carousel.getInstance(element)` |
| `getOrCreateInstance` | Static method which returns a carousel instance associated to a DOM element or create a new one in case it wasn't initialized. You can use it like this: `bootstrap.Carousel.getOrCreateInstance(element)` |
| `next` | Cycles to the next item. **Returns to the caller before the next item has been shown** (e.g., before the `slid.bs.carousel` event occurs). |
| `nextWhenVisible` | Don't cycle carousel to next when the page isn't visible or the carousel or its parent isn't visible. **Returns to the caller before the target item has been shown** |
| `pause` | Stops the carousel from cycling through items. |
| `prev` | Cycles to the previous item. **Returns to the caller before the previous item has been shown** (e.g., before the `slid.bs.carousel` event occurs). |
| `to` | Cycles the carousel to a particular frame (0 based, similar to an array). **Returns to the caller before the target item has been shown** (e.g., before the `slid.bs.carousel` event occurs). |
{{< /bs-table >}}

## Events

Bootstrap's carousel class exposes two events for hooking into carousel functionality. Both events have the following additional properties:

- `direction`: The direction in which the carousel is sliding (either `"left"` or `"right"`).
- `relatedTarget`: The DOM element that is being slid into place as the active item.
- `from`: The index of the current item
- `to`: The index of the next item

All carousel events are fired at the carousel itself (i.e. at the `<div class="carousel">`).

{{< bs-table >}}
| Event type | Description |
| --- | --- |
| `slid.bs.carousel` | Fired when the carousel has completed its slide transition. |
| `slide.bs.carousel` | Fires immediately when the `slide` instance method is invoked. |
{{< /bs-table >}}

```js
const myCarousel = document.getElementById('myCarousel')

myCarousel.addEventListener('slide.bs.carousel', event => {
  // do something...
})
```

{{</ tab >}}
{{</ tabs >}}

