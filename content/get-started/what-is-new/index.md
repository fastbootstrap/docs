---
layout: docs
title: What's New
seo_title: FastBootstrap Theme New Features
description: "Overview of our FastBootstrap theme, what's different from Bootstrap."
toc: true
icon: fa-solid fa-star
menu:
  get-started:    
weight: 60
---

FastBootstrap is a beautiful Bootstrap theme and extend a lot of Utilities CSS and components to help developers write less CSS, its fully compatible with Bootstrap 5.

If you want to migrate Bootstrap to new FastBootstrap, make sure to read this article before migrating.

## Bootstrap Spacers

The Bootstrap's `$spacers` maximum value is only `3rem`, and there are only 5 classes, which is not enough when we are designing.

### Margin

All of the "Margin" classes, including `mx-{value}`, `my-{value}`, `m{x|y}-{breakpoint}-{value}`. See the [Margin utilitie]({{< docsref "margin" >}}) for more Margin CSS.

{{< bs-table "table api-class-table" >}}
| Class | Bootstrap | FastBootstrap |
| --- | --- | --- |
| `.m-0` | 0 | 0 |
| `.m-1` | 0.25rem | 0.25rem |
| `.m-2` | 0.5rem | 0.5rem |
| `.m-3` | 1rem | 0.75rem |
| `.m-4` | 1.5rem | 1rem |
| `.m-5` | 3rem | 1.25rem |
| `.m-6` | - | 1.5rem | 
| `...` | - | ... |
{{</ bs-table >}}

### Padding

All of the "Padding" classes, including `px-{value}`, `py-{value}`, `p{x|y}-{breakpoint}-{value}`. See the [Padding utilitie]({{< docsref "padding" >}}) for more Padding CSS.

{{< bs-table "table api-class-table" >}}
| Class | Bootstrap | FastBootstrap |
| --- | --- | --- |
| `.p-0` | 0 | 0 |
| `.p-1` | 0.25rem | 0.25rem |
| `.p-2` | 0.5rem | 0.5rem |
| `.p-3` | 1rem | 0.75rem |
| `.p-4` | 1.5rem | 1rem |
| `.p-5` | 3rem | 1.25rem |
| `.p-6` | - | 1.5rem | 
| `...` | - | ... |
{{</ bs-table >}}

### Gap

All of the "Gap" classes, including `row-gap-{value}`, `column-{value}`, `gap-{breakpoint}-{value}`. See the [Gap utilitie]({{< docsref "gap" >}}) for more Gap CSS.

{{< bs-table "table api-class-table" >}}
| Class | Bootstrap | FastBootstrap |
| --- | --- | --- |
| `.gap-0` | 0 | 0 |
| `.gap-1` | 0.25rem | 0.25rem |
| `.gap-2` | 0.5rem | 0.5rem |
| `.gap-3` | 1rem | 0.75rem |
| `.gap-4` | 1.5rem | 1rem |
| `.gap-5` | 3rem | 1.25rem |
{{</ bs-table >}}