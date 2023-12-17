---
layout: docs
title: Transition Property
description: Utilities for controlling which CSS properties transition.
toc: true
group: transitions-animation
status: new
menu:
  docs:    
    weight: 10
---

## Quick reference

{{< class-api "transition-property" >}}

## Basic usage

### Controlling transitioned properties

Use the `transition-{properties}` utilities to specify which properties should transition when they change.

{{< callout info >}}
Hover each button to see the expected behaviour
{{</ callout >}}

{{< example class="bg-neutral-subtler bg-grid-slate-100 pb-10 text-center" show_source="false" >}}
  <button class="btn text-bg-discovery transition ease-in-out delay-150 -translate-y-px-hover duration-300 scale-110-hover">Save changes</button>  
{{</ example >}}

```html
<button class="transition ease-in-out delay-150 -translate-y-px-hover duration-300 scale-110-hover">Save changes</button>
```