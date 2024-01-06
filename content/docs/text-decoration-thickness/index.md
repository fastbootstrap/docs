---
layout: docs
title: Text Decoration Thickness
description: Utilities for controlling the thickness of text decorations.
toc: true
status: new
group: typography
menu:
  docs:    
---

## Quick reference

{{< class-api "text-decoration-thickness" >}}

## Basic usage

### Setting the text decoration thickness

Use the `decoration-{width}` utilities to change the thickness of an element’s [text decoration]({{< docsref "text-decoration" >}}).


{{< example class="bg-neutral-subtler bg-grid-slate-100" show_source="false" >}}
<div class="d-flex flex-column gap-4">
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-1</span>
    <p class="text-decoration-underline decoration-1 fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-2</span>
    <p class="text-decoration-underline decoration-2 fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted fs-sm fw-semibold text-body-tertiary mb-3">decoration-4</span>
    <p class="text-decoration-underline decoration-4 fs-5 fw-medium">The quick brown fox jumps over the lazy dog.</p>
  </div>
</div>
{{</ example >}}

```html
<p class="text-decoration-underline decoration-1 ...">The quick brown fox...</p>
<p class="text-decoration-underline decoration-2 ...">The quick brown fox...</p>
<p class="text-decoration-underline decoration-4 ...">The quick brown fox...</p>
```