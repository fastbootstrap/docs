---
layout: docs
title: Button Group
description: "Button group component is a grouping of buttons that gives users access to frequently performed, related actions."
toc: true
group: actions
menu:
  components:
---

**Bootstrap 5 Button group component**

Responsive button group built with the latest Bootstrap 5. Button group component is a series of buttons together on a single line or stacked together on a vertical column.

## Basic button group

Button groups display multiple buttons with evenly distributed spaces between them. Just wrap a series of buttons with `.btn` in `.btn-group`. 

{{< example >}}
<div class="btn-group" role="group" aria-label="Basic example">
  <button type="button" class="btn btn-primary">Left</button>
  <button type="button" class="btn btn-primary">Middle</button>
  <button type="button" class="btn btn-primary">Right</button>
</div>
{{</ example >}}

For an action or navigation into a line of text, these classes can also be added to links.

{{< example >}}
<div class="btn-group">
  <a href="#" class="btn btn-primary active" aria-current="page">Active link</a>
  <a href="#" class="btn btn-primary">Link</a>
  <a href="#" class="btn btn-primary">Link</a>
</div>
{{</ example >}}

{{< callout warning >}}

#### Ensure correct `role` and provide a label

In order for assistive technologies (such as screen readers) to convey that a series of buttons is grouped, an appropriate `role` attribute needs to be provided. For button groups, this would be `role="group"`, while toolbars should have a role="toolbar".

In addition, groups and toolbars should be given an explicit label, as most assistive technologies will otherwise not announce them, despite the presence of the correct `role` attribute. In the examples provided here, we use `aria-label`, but alternatives such as `aria-labelledby` can also be used.

{{</ callout >}}


## Outlined styles

Use the following button styles to show the colors only for the border of the element.

{{< example >}}
<div class="btn-group" role="group" aria-label="Basic outlined example">
  <button type="button" class="btn btn-outline-primary">Left</button>
  <button type="button" class="btn btn-outline-primary">Middle</button>
  <button type="button" class="btn btn-outline-primary">Right</button>
</div>
{{</ example >}}

## Checkbox and radio button groups

Combine button-like checkbox and radio toggle buttons into a seamless looking button group. There are 2 types of segmented buttons: `Single-select` and `Multi-select`.

### Single-select

Use a single-select segmented button with [Radio toggle button]({{< docsref "radio#radio-button-group" >}}) to select one option from a set, switch between views, or sort elements from up to five options. 

{{< example >}}
  <div class="btn-group" role="group" aria-label="Basic radio toggle button group">
    <input type="radio" class="btn-check" name="btnradio" id="btnradio1" autocomplete="off" checked />
    <label class="btn btn-default" for="btnradio1"><i class="fa-solid fa-align-left"></i></label>
    <input type="radio" class="btn-check" name="btnradio" id="btnradio2" autocomplete="off" />
    <label class="btn btn-default ms-0" for="btnradio2"><i class="fa-solid fa-align-center"></i></label>
    <input type="radio" class="btn-check" name="btnradio" id="btnradio3" autocomplete="off" />
    <label class="btn btn-default ms-0" for="btnradio3"><i class="fa-solid fa-align-right"></i></label>
    <input type="radio" class="btn-check" name="btnradio" id="btnradio4" autocomplete="off" />
    <label class="btn btn-default ms-0" for="btnradio4"><i class="fa-solid fa-align-justify"></i></label>
  </div>
{{</ example >}}

### Multi-select

Use a multi-select segmented button with [Checkbox toggle button]({{< docsref "checkbox#checkbox-button-group" >}}) to select or sort from two to five options. 

{{< example >}}
  <div class="btn-group" role="group" aria-label="Basic checkbox toggle button group">
    <input type="checkbox" class="btn-check" id="btncheck1" autocomplete="off" checked />
    <label class="btn btn-default" for="btncheck1"><i class="fa-solid fa-bold"></i></label>
    <input type="checkbox" class="btn-check" id="btncheck2" autocomplete="off" checked />
    <label class="btn btn-default" for="btncheck2"><i class="fa-solid fa-italic"></i></label>
    <input type="checkbox" class="btn-check" id="btncheck3" autocomplete="off" />
    <label class="btn btn-default" for="btncheck3"><i class="fa-solid fa-underline"></i></label>
    <input type="checkbox" class="btn-check" id="btncheck4" autocomplete="off" />
    <label class="btn btn-default" for="btncheck4"><i class="fa-solid fa-strikethrough"></i></label>
  </div>
{{</ example >}}

## Selected state

Adding an `.active` to `.btn` will keep the button in a selected state in the button group.

{{< example class="d-grid justify-content-start gap-4" >}}
<div class="btn-group" role="group" aria-label="Basic example">
  <button type="button" class="btn btn-default active">Day</button>
  <button type="button" class="btn btn-default">Week</button>
  <button type="button" class="btn btn-default">Month</button>
  <button type="button" class="btn btn-default">Year</button>
</div>
{{</ example >}}

## Button toolbar

Combine sets of button groups into button toolbars for more complex components.

{{< example >}}
<div class="btn-toolbar" role="toolbar" aria-label="Toolbar with button groups">
  <div class="btn-group" role="group" aria-label="First group">
    <button type="button" class="btn btn-primary">1</button>
    <button type="button" class="btn btn-primary">2</button>
    <button type="button" class="btn btn-primary">3</button>
    <button type="button" class="btn btn-primary">4</button>
  </div>
  <div class="btn-group ms-2" role="group" aria-label="Second group">
    <button type="button" class="btn btn-secondary">5</button>
    <button type="button" class="btn btn-secondary">6</button>
    <button type="button" class="btn btn-secondary">7</button>
  </div>
  <div class="btn-group ms-2" role="group" aria-label="Third group">
    <button type="button" class="btn btn-default">8</button>
  </div>
</div>
{{</ example >}}

Feel free to mix input groups with button groups in your toolbars. Similar to the example above, you’ll likely need some utilities to space things properly.

{{< example class="d-grid gap-3" >}}
<div class="btn-toolbar" role="toolbar">
  <div class="btn-group me-3" role="group" aria-label="First group">
    <button type="button" class="btn btn-outline-primary">1</button>
    <button type="button" class="btn btn-outline-primary">2</button>
    <button type="button" class="btn btn-outline-primary">3</button>
    <button type="button" class="btn btn-outline-primary">4</button>
  </div>
  <div class="input-group input-group-prefix">    
    <input type="text" class="form-control" placeholder="Input group example" 
    aria-label="Input group example" aria-describedby="btnGroupAddon">
    <div class="input-group-text">@</div>
  </div>
</div>

<div class="btn-toolbar justify-content-between" role="toolbar">
  <div class="btn-group me-3" role="group" aria-label="First group">
    <button type="button" class="btn btn-outline-primary">1</button>
    <button type="button" class="btn btn-outline-primary">2</button>
    <button type="button" class="btn btn-outline-primary">3</button>
    <button type="button" class="btn btn-outline-primary">4</button>
  </div>
  <div class="input-group input-group-prefix">
    <input type="text" class="form-control" placeholder="Input group example" 
    aria-label="Input group example" aria-describedby="btnGroupAddon2">
    <div class="input-group-text">@</div>
  </div>
</div>
{{</ example >}}

## Sizes

Instead of applying button sizing classes to every button in a group, just add `.btn-group-{lg|sm}` to each `.btn-group` or `.btn-group`, including each one when nesting multiple groups.

{{< example class="d-grid gap-4 auto-cols-min justify-content-start" >}}
<div class="btn-group btn-group-lg" role="group" aria-label="Large button group">
  <button type="button" class="btn btn-default">Left</button>
  <button type="button" class="btn btn-default">Middle</button>
  <button type="button" class="btn btn-default">Right</button>
</div>
<div class="btn-group" role="group" aria-label="Default button group">
  <button type="button" class="btn btn-default">Left</button>
  <button type="button" class="btn btn-default">Middle</button>
  <button type="button" class="btn btn-default">Right</button>
</div>
<div class="btn-group btn-group-sm" role="group" aria-label="Small button group">
  <button type="button" class="btn btn-default">Left</button>
  <button type="button" class="btn btn-default">Middle</button>
  <button type="button" class="btn btn-default">Right</button>
</div>
{{</ example >}}

## Colors

Use the `.btn-{color}` to control the appearance of the button in the button group.

{{< example class="d-grid gap-3 auto-cols-min justify-content-start" >}}
<div class="btn-group" role="group">
  <button type="button" class="btn btn-default">Left</button>
  <button type="button" class="btn btn-default">Middle</button>
  <button type="button" class="btn btn-default">Right</button>
</div>
<div class="btn-group" role="group">
  <button type="button" class="btn btn-primary">Left</button>
  <button type="button" class="btn btn-primary">Middle</button>
  <button type="button" class="btn btn-primary">Right</button>
</div>
<div class="btn-group" role="group">
  <button type="button" class="btn btn-danger">Left</button>
  <button type="button" class="btn btn-danger">Middle</button>
  <button type="button" class="btn btn-danger">Right</button>
</div>
<div class="btn-group" role="group">
  <button type="button" class="btn btn-success">Left</button>
  <button type="button" class="btn btn-success">Middle</button>
  <button type="button" class="btn btn-success">Right</button>
</div>
{{</ example >}}


## Vertically stacked group

Use the `.btn-group-vertical` to make a set of buttons appear vertically stacked rather than horizontally. 

{{< example >}}
<div class="btn-group-vertical" role="group" aria-label="Vertical button group">
  <button type="button" class="btn btn-primary">Button 1</button>
  <button type="button" class="btn btn-primary">Button 2</button>
  <button type="button" class="btn btn-primary">Button 3</button>
  <button type="button" class="btn btn-primary">Button 4</button>
  <button type="button" class="btn btn-primary">Button 5</button>
</div>
{{</ example >}}

You can also nest dropdown elements inside button groups.

{{< example >}}
<div class="btn-group-vertical" role="group" aria-label="Vertical button group">
  <button type="button" class="btn btn-primary">Button</button>
  <button type="button" class="btn btn-primary">Button</button>
  <div class="btn-group" role="group">
    <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
      Dropdown
    </button>
    <ul class="dropdown-menu">
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
    </ul>
  </div>
  <div class="btn-group dropstart" role="group">
    <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
      Dropdown
    </button>
    <ul class="dropdown-menu">
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
    </ul>
  </div>
  <div class="btn-group dropend" role="group">
    <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
      Dropdown
    </button>
    <ul class="dropdown-menu">
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
    </ul>
  </div>
  <div class="btn-group dropup" role="group">
    <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
      Dropdown
    </button>
    <ul class="dropdown-menu">
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
      <li><a class="dropdown-item" href="#">Dropdown link</a></li>
    </ul>
  </div>
</div>
{{</ example >}}

## Nesting group

Place a `.btn-group` within another `.btn-group` when you want dropdown menus mixed with a series of buttons.

{{< example >}}
<div class="btn-toolbar">
  <div class="btn-group" role="group" aria-label="Button group with nested dropdown">
    <button type="button" class="btn btn-primary">1</button>
    <button type="button" class="btn btn-primary">2</button>
    <div class="btn-group" role="group">
      <button type="button" class="btn btn-primary dropdown-toggle"
       data-bs-toggle="dropdown" aria-expanded="false">Dropdown</button>
      <ul class="dropdown-menu">
        <li><a class="dropdown-item" href="#">Dropdown link</a></li>
        <li><a class="dropdown-item" href="#">Dropdown link</a></li>
      </ul>
    </div>
    <button type="button" class="btn btn-primary">3</button>
  </div>
</div>
{{</ example >}}
