---
layout: docs
title: Icon Color
description: "Utilities for controlling the color of icon."
toc: true
group: icon
status: new
menu:
  docs:    
    weight: 100
---

## Quick reference 


{{< colors.inline >}}
<table class="table api-class-table">
  <thead>
    <tr>
      <th>Class</th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    {{ range (index $.Site.Data.css "icon-color" ) }}
      {{ $prefix := .class }}
      {{ range .values }} 
        {{ $key := . }}
        {{ $value := . }}
        {{ if reflect.IsMap . }}
          {{ range $key, $value = . }}
          {{ end }}
        {{ end }}
        <tr>
          <td><code>{{ printf "%s-%s" $prefix $key }}</code></td>
          <td class="fw-semibold"><span class="{{ $value }}">Aa</span></td>
        </tr>
      {{ end }}
    {{ end }}
  </tbody>
</table>
{{< / colors.inline >}}

{{< callout info >}}
`icon-{color}` supports dark mode unlike `text-{color}` just one color even in the dark mode.
{{</ callout >}}

## Basic usage

### Setting the icon color 

Control the text color of an icon using the `icon-{color}` utilities.

{{< example class="bg-grid-slate-100 text-center">}}
<i class="fa-solid fa-bell fa-3x icon-primary"></i>
{{</ example >}}

In the dark Mode

{{< example class="p-0" show_source="false">}}
<div class="p-6 text-center" data-bs-theme="dark" >
<i class="fa-solid fa-bell fa-3x icon-primary"></i>
</div>
{{</ example >}}
