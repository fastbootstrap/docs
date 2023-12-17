---
layout: docs
title: Flex
description: "Utilities for controlling how flex items both grow and shrink."
toc: true
group: flexbox
menu:
  docs:
    weight: 70
---

Use the `.flex-fill` class on a series of sibling elements to force them into widths equal to their content (or equal widths if their content does not surpass their border-boxes) while taking up all available horizontal space.

## Quick reference

{{< class-api "flex" >}}

## Basic usage

### Flex 1

Use `flex-1` to allow a flex item to grow and shrink as needed, ignoring its initial size:

{{< example show_source="false" >}}
<div class="d-flex gap-4 bg-striped-teal rounded">
  <div class="p-4 d-flex flex-none align-items-center justify-content-center rounded text-bg-purple bd-w-14 bd-h-14">01</div>
  <div class="p-4 d-flex flex-1 align-items-center justify-content-center rounded text-bg-primary bd-w-64">02</div>
  <div class="p-4 d-flex flex-1 align-items-center justify-content-center rounded text-bg-primary bd-w-32">03</div>
</div>
{{</ example >}}

```html
<div class="d-flex">
  <div class="flex-none ...">01</div>
  <div class="flex-1 col-8 ...">02</div>
  <div class="flex-1 col-4 ...">03</div>
</div>
```

### Auto

Use `.flex-fill` to allow a flex item to grow and shrink, taking into account its initial size:

{{< example show_source="false" >}}
<div class="d-flex gap-4 bg-striped-purple rounded">
  <div class="d-flex flex-none align-items-center bd-w-14 bd-h-14 justify-content-center rounded text-bg-dark">01</div>
  <div class="d-flex flex-fill align-items-center justify-content-center rounded text-bg-purple col-8">02</div>
  <div class="d-flex flex-fill align-items-center justify-content-center rounded text-bg-purple col-4">03</div>
</div>
{{</ example >}}

```html
<div class="d-flex">
  <div class="flex-none ...">01</div>
  <div class="flex-fill col-8 ...">02</div>
  <div class="flex-fill col-4 ...">03</div>
</div>
```

## None

Use `flex-none` to prevent a flex item from growing or shrinking:

{{< example show_source="false" >}}
<div class="d-flex gap-4 bg-striped-purple rounded">
  <div class="d-flex flex-none align-items-center bd-w-14 bd-h-14 justify-content-center rounded bg-success-subtle">01</div>
  <div class="d-flex flex-none align-items-center justify-content-center rounded text-bg-success col-8">02</div>
  <div class="d-flex flex-1 align-items-center justify-content-center rounded text-bg-success col-4">03</div>
</div>
{{</ example >}}

```html
<div class="d-flex">
  <div class="flex-none ...">01</div>
  <div class="flex-none ...">02</div>
  <div class="flex-1 ...">03</div>
</div>
```

## Breakpoints

The `flex-fill` utilities that supports responsive at specific [breakpoints]({{< docsref "breakpoints" >}}), from `xs` to `xxl`, have no breakpoint abbreviation in them. 

The responsive classes are named using the format `flex-{breakpoint}-fill`.


{{< markdown >}}
{{< flex.inline >}}
{{- range $.Site.Data.breakpoints }}
{{- if ne .abbr "" }}
- `.flex{{ .abbr }}-fill`
{{- end -}}
{{- end -}}
{{< /flex.inline >}}
{{< /markdown >}}

For example, use `flex-md-fill` to apply the `flex-fill` utility at only medium screen sizes and above.

```html
<div class="d-flex flex-md-fill">
  <!-- ... -->
</div>
```