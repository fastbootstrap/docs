---
layout: docs
title: Text Decoration Color
description: Utilities for controlling the color of text decorations.
toc: true
status: new
group: typography
menu:
  docs:    
---

## Quick reference

{{< class-api "text-decoration-color" >}}

## Basic usage
​
### Setting the text decoration color

Use the `decoration-{color}` utilities to change the color of an element’s [text decoration]({{< docsref "text-decoration" >}}).

{{< example show_source="false" class="bg-neutral-subtler bg-grid-slate-100" >}}
<div class="max-w-sm mx-auto p-8 bg-body text-body shadow">
  <p>
    I’m Derek, an astro-engineer based in Tattooine. I like to build X-Wings at
    <a class="text-decoration-underline decoration-primary fw-semibold text-dark">My Company, Inc</a>.
    Outside of work, I like to <a class="text-decoration-underline decoration-danger  fw-semibold text-dark">watch
    pod-racing</a> and have <a class="text-decoration-underline decoration-warning  fw-semibold text-dark">light-saber</a> fights.
  </p>
</div>
{{</ example >}}

```html
<div>
  <p>
    I’m Derek, an astro-engineer based in Tattooine. I like to build X-Wings at
    <a class="text-decoration-underline decoration-primary">My Company, Inc</a>.
    Outside of work, I like to <a class="text-decoration-underline decoration-danger">watch
    pod-racing</a> and have <a class="text-decoration-underline decoration-warning">light-saber</a> fights.
  </p>
</div>
```