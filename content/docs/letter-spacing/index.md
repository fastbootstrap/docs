---
layout: docs
title: Letter Spacing
description: "Utilities for controlling the tracking (letter spacing) of an element."
toc: true
status: new
group: typography
menu:
  docs:    
---

## Quick reference

{{< class-api "letter-spacing" >}}

## Usage

### Setting the letter spacing

Control the letter spacing of an element using the `tracking-{size}` utilities.

{{< example class="bg-grid-slate-100" show_source="false" >}}
<div class="d-flex gap-4 flex-column">
  <div>
    <span class="text-muted mb-3 fs-sm fw-semibold">tracking-tight</span>
    <p class="tracking-tight fw-semibold fs-5">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted mb-3 fs-sm fw-semibold">tracking-normal</span>
    <p class="tracking-normal fw-semibold fs-5">The quick brown fox jumps over the lazy dog.</p>
  </div>
  <div>
    <span class="text-muted mb-3 fs-sm fw-semibold">tracking-wide</span>
    <p class="tracking-wide fw-semibold fs-5">The quick brown fox jumps over the lazy dog.</p>
  </div>
</div>
{{</ example >}}

```html
<p class="tracking-tight ...">The quick brown fox ...</p>
<p class="tracking-normal ...">The quick brown fox ...</p>
<p class="tracking-wide ...">The quick brown fox ...</p>
```