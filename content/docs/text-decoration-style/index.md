---
layout: docs
title: Text Decoration Style
description: Utilities for controlling the style of text decorations.
toc: true
status: new
group: typography
menu:
  docs:    
---

## Quick reference

{{< class-api "text-decoration-style" >}}

## Basic usage
​
### Setting the text decoration style

Use the `decoration-{style}` utilities to change the style of an element’s [text decoration]({{< docsref "text-decoration" >}}).


{{< example class="bg-neutral-subtler bg-grid-slate-100" show_source="false" >}}
<div class="d-flex flex-column gap-4">
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-solid</span>
    <p class="text-decoration-underline decoration-solid fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-double</span>
    <p class="text-decoration-underline decoration-double fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-dotted</span>
    <p class="text-decoration-underline decoration-dotted fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-dashed</span>
    <p class="text-decoration-underline decoration-dashed fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-wavy</span>
    <p class="text-decoration-underline decoration-wavy fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
</div>
{{</ example >}}

```html
<p class="text-decoration-underline decoration-solid ...">The quick brown fox...</p>
<p class="text-decoration-underline decoration-double ...">The quick brown fox...</p>
<p class="text-decoration-underline decoration-dotted ...">The quick brown fox...</p>
<p class="text-decoration-underline decoration-dashed ...">The quick brown fox...</p>
<p class="text-decoration-underline decoration-wavy ...">The quick brown fox...</p>
```