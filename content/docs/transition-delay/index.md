---
layout: docs
title: Transition Delay
description: Utilities for controlling the delay of CSS transitions.
toc: true
group: transitions-animation
status: new
menu:
  docs:    
    weight: 40
---

## Quick reference

{{< class-api "transition-delay" >}}

## Basic usage

### Delaying transitions

Use the `delay-{amount}` utilities to control an element’s transition-delay.

{{< callout info >}}
Hover each button to see the expected behaviour
{{</ callout >}}

{{< example class="bg-neutral-subtler bg-grid-slate-100 text-center" show_source="false" >}}
<div class="d-flex flex-wrap gap-5 justify-content-around">
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">delay-150</p>
    <button class="btn text-bg-primary transition delay-150 scale-125-hover duration-300 ease-in-out">Button A</button>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">delay-300</p>
    <button class="btn text-bg-primary transition delay-300 scale-125-hover duration-300 ease-in-out">Button B</button>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-4">delay-700</p>
    <button class="btn text-bg-primary transition delay-700 scale-125-hover duration-300 ease-in-out">Button C</button>
  </div>
</div>
{{</ example >}}

```html
<button class="transition delay-150 duration-300 ease-in-out ...">Button A</button>
<button class="transition delay-300 duration-300 ease-in-out ...">Button B</button>
<button class="transition delay-700 duration-300 ease-in-out ...">Button C</button>
```