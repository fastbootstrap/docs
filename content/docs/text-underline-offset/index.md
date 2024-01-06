---
layout: docs
title: Text Underline Offset
description: "Utilities for controlling the offset of a text underline."
toc: true
status: new
group: typography
menu:
  docs:
---

## Quick reference

{{< class-api "text-underline-offset" >}}

## Basic usage

### Setting the underline offset

Use the `underline-offset-{width}` utilities to change the offset of a text underline.

{{< example class="bg-neutral-subtler bg-grid-slate-100" show_source="false" >}}
<div class="d-flex flex-column gap-4">
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">underline-offset-1</span>
    <p class="text-decoration-underline underline-offset-1 fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">underline-offset-2</span>
    <p class="text-decoration-underline underline-offset-2 fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">underline-offset-4</span>
    <p class="text-decoration-underline underline-offset-4 fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">underline-offset-8</span>
    <p class="text-decoration-underline underline-offset-8 fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
</div>
{{</ example >}}

```html
<p class="text-decoration-underline underline-offset-1 ...">The quick brown fox...</p>
<p class="text-decoration-underline underline-offset-2 ...">The quick brown fox...</p>
<p class="text-decoration-underline underline-offset-4 ...">The quick brown fox...</p>
<p class="text-decoration-underline underline-offset-8 ...">The quick brown fox...</p>
```