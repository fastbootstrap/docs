---
layout: docs
title: Link
description: "Links allow users to navigate to a different location."
toc: true
group: utilities
menu:
  components:
aliases:
 - /docs/link
---

## Basic link

The example below a link with default behavior.

{{< example>}}
<div class="d-flex flex-column">
  <a href="#">Default link</a>
</div>
{{</ example >}}

## Colored links

You can use the `.link-*` classes to colorize links. Unlike the `.text-*` classes, these classes have a `:hover` and `:focus` state.

{{< example class="d-flex flex-column gap-2">}}
<a href="#" class="link-primary">Primary link</a>
<a href="#" class="link-secondary">Secondary link</a>
<a href="#" class="link-success">Success link</a>
<a href="#" class="link-danger">Danger link</a>
<a href="#" class="link-warning">Warning link</a>
<a href="#" class="link-info">Info link</a>
<a href="#" class="link-light">Light link</a>
<a href="#" class="link-dark">Dark link</a>
<a href="#" class="link-body-emphasis">Emphasis link</a>
{{</ example >}}

### Reset link color

Reset a link’s color with `.text-reset`, so that it inherits the color from its parent.

{{< example >}}
<p class="text-danger">
  Muted text with a <a href="#" class="text-reset">reset link</a>.
</p>
{{</ example >}}

## Link opacity

The below table are available CSS utilities for link opacity.

{{< bs-table "table api-class-table" >}}
| CSS | Desc |
| --- | --- |
| `.link-opacity-10` | --bs-link-opacity: .1 |
| `.link-opacity-25` | --bs-link-opacity: .25 |
| `.link-opacity-50` | --bs-link-opacity: .5 |
| `.link-opacity-75` | --bs-link-opacity: .75 |
| `.link-opacity-100` | --bs-link-opacity: 100 |
{{< /bs-table >}}

{{< example class="d-flex flex-wrap gap-3" >}}
<a class="link-opacity-25" href="#">Link 1</a>
<a class="link-opacity-75" href="#">Link 2</a>
<a class="link-opacity-100" href="#">Link 3</a>
{{</ example >}}

You can even change the opacity level on `hover` by `.link-opacity-*-hover`.

{{< example class="d-flex flex-wrap gap-3" >}}
<a class="link-opacity-10-hover" href="#">Link 1</a>
<a class="link-opacity-75-hover" href="#">Link 2</a>
<a class="link-opacity-100-hover" href="#">Link 3</a>
{{</ example >}}

## Link underlines 

Add a `.link-underline` to the link element to display underline.

{{< example >}}
<a href="#" class="link-underline">Underline link</a>
{{</ example >}}

### Underline color

Change the underline’s color independent of the link text color by `.link-underline-{color}`.

{{< example class="d-flex flex-column gap-2" >}}
<a href="#" class="link-underline-primary">Primary underline</a>
<a href="#" class="link-underline-secondary">Secondary underline</a>
<a href="#" class="link-underline-success">Success underline</a>
<a href="#" class="link-underline-danger">Danger underline</a>
<a href="#" class="link-underline-warning">Warning underline</a>
<a href="#" class="link-underline-info">Info underline</a>
<a href="#" class="link-underline-light">Light underline</a>
<a href="#" class="link-underline-dark">Dark underline</a>
{{</ example >}}

### Underline offset 

Change the underline’s distance from your text. Offset is set in `em` units to automatically scale with the element’s current `font-size`.

{{< example class="d-flex flex-column gap-2" >}}
<a class="link-underline" href="#">Default link</a>
<a class="link-underline link-offset-1" href="#">Offset 1 link</a>
<a class="link-underline link-offset-2" href="#">Offset 2 link</a>
<a class="link-underline link-offset-3" href="#">Offset 3 link</a>
{{</ example >}}

### Underline opacity


{{< bs-table "table api-class-table" >}}
| CSS | Desc |
| --- | --- |
| `.link-underline-opacity-10` | --bs-link-underline-opacity: .1 |
| `.link-underline-opacity-25` | --bs-link-underline-opacity: .25 |
| `.link-underline-opacity-50` | --bs-link-underline-opacity: .5 |
| `.link-underline-opacity-75` | --bs-link-underline-opacity: .75 |
| `.link-underline-opacity-100` | --bs-link-underline-opacity: 100 |
{{< /bs-table >}}

{{< example class="d-flex flex-column gap-3" >}}
<a href="#" class="link-primary link-underline link-underline-opacity-25 link-underline-opacity-100-hover">Primary link</a>
<a href="#" class="link-secondary link-underline link-underline-opacity-25 link-underline-opacity-100-hover">Secondary link</a>
{{</ example >}}

### Hover variants

ust like the `.link-opacity-*-hover` utilities, `.link-offset` and `.link-underline-opacity` utilities include `:hover` variants by default. Mix and match to create unique link styles.

{{< example >}}
<a class="link-offset-2 link-offset-3-hover link-underline link-underline-opacity-0 link-underline-opacity-75-hover" href="#">
  Underline opacity 0
</a>
{{</ example >}}

## No underline 

Use the [text decoration utilities]({{< docsref "text-decoration" >}}) `text-decoration-none` to remove the underline when mouse hover a link.

{{< example>}}
<div class="d-flex flex-column">
  <a href="#" class="text-decoration-none">This ia a link</a>
</div>
{{</ example >}}

## Related

- [Stretched Link]({{< docsref "stretched-link" >}})