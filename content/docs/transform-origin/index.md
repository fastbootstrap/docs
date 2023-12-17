---
layout: docs
title: Transform Origin
description: "Utilities for specifying the origin an element with transformations."
toc: true
group: transforms
status: new
menu:
  docs:    
    weight: 50
---

## Quick reference

{{< class-api "origin" >}}

## Basic usage
​
### Changing the transform origin

Specify an element’s transform origin using the `origin-{keyword}` utilities.


{{< example class="bg-neutral-subtler bg-grid-slate-100 pb-10 text-center" show_source="false" >}}
<div class="d-flex flex-wrap gap-5 justify-content-around">
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">origin-center</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="origin-center rotate-45 z-10">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">origin-top-left</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="origin-top-left rotate-12 z-10 position-relative">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
  <div class="d-flex flex-column align-items-center">
    <p class="text-body-tertiary fw-medium fs-sm mb-6 mb-lg-9">origin-bottom</p>
    <div class="position-relative">
      <div class="position-absolute">
        <img class="bd-w-24 bd-h-24 rounded opacity-25"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
      <div class="origin-bottom -rotate-12 z-10 position-relative">
        <img class="bd-w-24 bd-h-24 rounded"
          src="https://images.unsplash.com/photo-1554629947-334ff61d85dc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=320&h=320&q=80" />
      </div>
    </div>
  </div>
</div>
{{</ example >}}