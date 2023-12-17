---
layout: docs
title: Skew
description: "Utilities for skewing elements with transform."
toc: true
group: transforms
status: new
menu:
  docs:    
    weight: 40
---

## Quick reference

{{< class-api "skew" >}}

## Basic usage
​
### Skewing an element

Use the `skew-x-{amount}` and `skew-y-{amount}` utilities to skew an element.


{{< example class="bg-neutral-subtler bg-grid-slate-100 pb-10 text-center" show_source="false" >}}
<div class="d-flex flex-wrap gap-5 justify-content-around">
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">skew-y-0</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="skew-y-0 z-10">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">skew-y-3</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="skew-y-3 z-10 position-relative">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">skew-y-6</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="skew-y-6 z-10 position-relative">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">skew-y-12</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="skew-y-12 z-10 position-relative">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
</div>
{{</ example >}}

```html
<img class="skew-y-0 ...">
<img class="skew-y-3 ...">
<img class="skew-y-6 ...">
<img class="skew-y-12 ...">
```

### Using negative values

To use a negative skew value, prefix the class name with a dash to convert it to a negative value.

```html
<img class="-skew-y-6 ...">
```

### Removing transforms

To remove all of the transforms on an element at once, use the `transform-none` utility:

```html
<div class="scale-75 translate-x-4 skew-y-3 transform-none">
  <!-- ... -->
</div>
```
