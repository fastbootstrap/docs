---
layout: docs
title: Space Between
description: Utilities for controlling the space between child elements.
toc: true
group: Spacing
menu:
  docs:    
---

Use the Bootstrap's [Gaps]({{< docsref "gap" >}}) utilitie to controlling the space between child elements.

## Quick reference

{{< class-api "gap" true >}}

## Basic usage

### Add horizontal space between children

Control the horizontal space between elements using the `column-gap-{amount}` utilities.

{{< example class="bg-grid-slate-100" show_source="false" >}}
<div class="d-flex column-gap-4 bg-striped-purple rounded max-w-fit">
  <div class="bd-w-14 bd-h-14 d-flex align-items-center justify-content-center rounded text-center text-bg-purple fw-semibold">01</div>
  <div class="bd-w-14 bd-h-14 d-flex align-items-center justify-content-center  rounded text-center text-bg-purple fw-semibold">02</div>
  <div class="bd-w-14 bd-h-14 d-flex align-items-center justify-content-center rounded text-center text-bg-purple fw-semibold">03</div>
</div>
{{</ example >}}

```html
<div class="d-flex column-gap-4 ...">
  <div>01</div>
  <div>02</div>
  <div>03</div>
</div>
```

## Add vertical space between children

Control the vertical space between elements using the `row-gap-{amount}` utilities.


{{< example class="bg-grid-slate-100" show_source="false" >}}
<div class="d-flex flex-column row-gap-4 bg-striped-purple rounded">
  <div class=" bd-h-14 d-flex align-items-center justify-content-center rounded text-center text-bg-primary fw-semibold">01</div>
  <div class="bd-h-14 d-flex align-items-center justify-content-center  rounded text-center  text-bg-primary fw-semibold">02</div>
  <div class="bd-h-14 d-flex align-items-center justify-content-center rounded text-center text-bg-primary fw-semibold">03</div>
</div>
{{</ example >}}

```html
<div class="d-flex flex-column row-gap-4 ...">
  <div>01</div>
  <div>02</div>
  <div>03</div>
</div>
```

### Reversing children order

Using the [.flex-row-reverse]({{< docsref "flex-direction" >}}) utilite to reversing the children elements.

{{< example class="bg-grid-slate-100" show_source="false" >}}
<div class="d-flex justify-content-end">
<div class="d-flex flex-row-reverse column-gap-4 bg-striped-purple rounded max-w-fit">
  <div class="bd-w-14 bd-h-14 d-flex align-items-center justify-content-center rounded text-center text-bg-purple fw-semibold">01</div>
  <div class="bd-w-14 bd-h-14 d-flex align-items-center justify-content-center  rounded text-center text-bg-purple fw-semibold">02</div>
  <div class="bd-w-14 bd-h-14 d-flex align-items-center justify-content-center rounded text-center text-bg-purple fw-semibold">03</div>
</div>
</div>
{{</ example >}}

```html
<div class="d-flex flex-row-reverse column-gap-4 ...">
  <div>01</div>
  <div>02</div>
  <div>03</div>
</div>
```
## Breakpoints and media queries

All utilities that supports responsive at specific breakpoints, from `xs` to `xxl`, have no breakpoint abbreviation in them.

```html
<div class="d-flex column-gap-4 column-gap-lg-6...">
  <div>01</div>
  <div>02</div>
  <div>03</div>
</div>
```