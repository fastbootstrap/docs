---
layout: docs
title: Transition Duration
description: Utilities for controlling the duration of CSS transitions.
toc: true
group: transitions-animation
status: new
menu:
  docs:    
    weight: 20
---

## Quick reference

{{< class-api "transition-duration" >}}

## Basic usage

### Changing transition duration

Use the `duration-{amount}` utilities to control an element’s transition-duration.

{{< callout info >}}
Hover each button to see the expected behaviour
{{</ callout >}}

{{< example class="bg-neutral-subtler bg-grid-slate-100 text-center" show_source="false" >}}
<div class="d-flex flex-wrap gap-5 justify-content-around">
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">duration-150</p>
    <button class="btn text-bg-primary transition scale-125-hover duration-150 ease-in-out">Button A</button>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">duration-300</p>
    <button class="btn text-bg-primary transition scale-125-hover duration-300 ease-in-out">Button B</button>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">duration-700</p>
    <button class="btn text-bg-primary transition scale-125-hover duration-700 ease-in-out">Button C</button>
  </div>
</div>
{{</ example >}}

```html
<button class="ease-in duration-300 ...">Button A</button>
<button class="ease-out duration-300 ...">Button B</button>
<button class="ease-in-out duration-300 ...">Button C</button>
```