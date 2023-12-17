---
layout: docs
title: Scale
description: "Utilities for scaling elements with transform."
toc: true
group: transforms
status: new
menu:
  docs:    
    weight: 10
---

## Quick reference

{{< class-api "scale" true >}}

## Basic usage

### Scaling an element

Use the `scale-{percentage}`, `scale-x-{percentage}`, and `scale-y-{percentage}` utilities to scale an element.

{{< example class="bg-neutral-subtler bg-grid-slate-100 pb-10 text-center" show_source="false" >}}
<div class="d-flex flex-wrap gap-5 justify-content-around">
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">scale-75</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="scale-75 z-10">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">scale-100</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="scale-100 z-10 position-relative">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">scale-125</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="scale-125 z-10 position-relative">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
</div>
{{</ example >}}

```html
<img class="scale-75 ...">
<img class="scale-100 ...">
<img class="scale-125 ...">
```

### Removing transforms

To remove all of the transforms on an element at once, use the transform-none utility:

```html
<div class="scale-75 translate-x-4 skew-y-3 transform-none">
  <!-- ... -->
</div>
```

## Hover state

The utility classes supports **hover** states, using the following format `.scale-{percentage}-{x|y}-hover`. For example, use `scale-125-hover` to only apply the `scale-125 ` utility on hover.

```html
<div class="scale-125-hover">
  <!-- ... -->
</div>
```