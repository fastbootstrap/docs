---
layout: docs
title: Transition Timing Function
description: Utilities for controlling the easing of CSS transitions.
toc: true
group: transitions-animation
status: new
menu:
  docs:    
    weight: 30
---

## Quick reference

{{< class-api "transition-timing-function" >}}

## Basic usage

### Controlling the easing curve

Use the `ease-{timing}` utilities to control an element’s easing curve.

{{< callout info >}}
Hover each button to see the expected behaviour
{{</ callout >}}

{{< example class="bg-neutral-subtler bg-grid-slate-100 text-center" show_source="false" >}}
<div class="d-flex flex-wrap gap-5 justify-content-around">
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">ease-in</p>
    <button class="btn text-bg-primary transition scale-125-hover duration-300 ease-in">Button A</button>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">ease-out</p>
    <button class="btn text-bg-primary transition scale-125-hover duration-300 ease-out">Button B</button>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">ease-in-out</p>
    <button class="btn text-bg-primary transition scale-125-hover duration-300 ease-in-out">Button C</button>
  </div>
</div>
{{</ example >}}

```html
<button class="ease-in duration-300 ...">Button A</button>
<button class="ease-out duration-300 ...">Button B</button>
<button class="ease-in-out duration-300 ...">Button C</button>
```