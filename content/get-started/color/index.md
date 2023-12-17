---
layout: docs
title: Color System
description: "Our color system is based on a Atlassian design color foundation that designed for our components and element styles."
toc: true
menu:
  get-started:    
icon: fa-solid fa-fill-drip
weight: 50
aliases:
  - /docs/color
---

Bootstrap is supported by an extensive color system that themes our styles and components. This enables more comprehensive customization and extension for any project.

## Colors

Bootstrap colors ending in `-rgb` provide the `red`, `green`, `blue` values for use in `rgb()` and `rgba()` color modes. For example, `rgba(var(--bs-secondary-bg-rgb), .5)`.
<div class="table-responsive">
  <table class="table">
    <thead>
      <tr>
        <th style="width: 340px;">Description</th>
        <th style="width: 200px;">Swatch</th>
        <th>Variables</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td rowspan="2" class="align-top"><strong>Body —</strong> Default foreground (color) and background, including components.</td>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-body-color);">&nbsp;</div>
        </td>
        <td><code>--bs-body-color</code><br /><code>--bs-body-color-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2 border" style="background-color: var(--bs-body-bg);">&nbsp;</div>
        </td>
        <td><code>--bs-body-bg</code><br /><code>--bs-body-bg-rgb</code></td>
      </tr>
      <tr>
        <td rowspan="2" class="align-top"><strong>Secondary —</strong> Use the <code>color</code> option for lighter text. Use the <code>bg</code> option for dividers and to indicate disabled component states.</td>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-secondary-color);">&nbsp;</div>
        </td>
        <td><code>--bs-secondary-color</code><br /><code>--bs-secondary-color-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2 border" style="background-color: var(--bs-secondary-bg);">&nbsp;</div>
        </td>
        <td><code>--bs-secondary-bg</code><br /><code>--bs-secondary-bg-rgb</code></td>
      </tr>
      <tr>
        <td rowspan="2" class="align-top">
          <strong>Tertiary —</strong> Use the <code>color</code> option for even lighter text. Use the <code>bg</code>
          option to style backgrounds for hover states, accents, and wells.
        </td>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-tertiary-color);">&nbsp;</div>
        </td>
        <td><code>--bs-tertiary-color</code><br /><code>--bs-tertiary-color-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2 border" style="background-color: var(--bs-tertiary-bg);">&nbsp;</div>
        </td>
        <td><code>--bs-tertiary-bg</code><br /><code>--bs-tertiary-bg-rgb</code></td>
      </tr>
      <tr>
        <td><strong>Emphasis —</strong> For higher contrast text. Not applicable for backgrounds.</td>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-emphasis-color);">&nbsp;</div>
        </td>
        <td><code>--bs-emphasis-color</code><br /><code>--bs-emphasis-color-rgb</code></td>
      </tr>
      <tr>
        <td><strong>Border —</strong> For component borders, dividers, and rules. Use <code>--bs-border-color-translucent</code> to blend with backgrounds with an <code>rgba()</code> value.</td>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-border-color);">&nbsp;</div>
        </td>
        <td><code>--bs-border-color</code><br /><code>--bs-border-color-rgb</code></td>
      </tr>
      <tr>
        <td rowspan="4" class="align-top"><strong>Primary —</strong> Main theme color, used for hyperlinks, focus styles, and component and form active states.</td>
        <td>
          <div class="p-3 rounded-2 bg-primary">&nbsp;</div>
        </td>
        <td><code>--bs-primary</code><br /><code>--bs-primary-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-primary-bg-subtle)">&nbsp;</div>
        </td>
        <td>
          <code>--bs-primary-bg-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="border: 5px var(--bs-primary-border-subtle) solid">&nbsp;</div>
        </td>
        <td>
          <code>--bs-primary-border-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="py-3 fw-bold h5" style="color: var(--bs-primary-text-emphasis)">Text</div>
        </td>
        <td>
          <code>--bs-primary-text-emphasis</code>
        </td>
      </tr>
      <tr>
        <td rowspan="4" class="align-top"><strong>Success —</strong> Theme color used for positive or successful actions and information.</td>
        <td>
          <div class="p-3 rounded-2 bg-success">&nbsp;</div>
        </td>
        <td><code>--bs-success</code><br /><code>--bs-success-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-success-bg-subtle)">&nbsp;</div>
        </td>
        <td>
          <code>--bs-success-bg-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="border: 5px var(--bs-success-border-subtle) solid">&nbsp;</div>
        </td>
        <td>
          <code>--bs-success-border-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="py-3 fw-bold h5" style="color: var(--bs-success-text-emphasis)">Text</div>
        </td>
        <td>
          <code>--bs-success-text-emphasis</code>
        </td>
      </tr>
      <tr>
        <td rowspan="4" class="align-top"><strong>Danger —</strong> Theme color used for errors and dangerous actions.</td>
        <td>
          <div class="p-3 rounded-2 bg-danger">&nbsp;</div>
        </td>
        <td><code>--bs-danger</code><br /><code>--bs-danger-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-danger-bg-subtle)">&nbsp;</div>
        </td>
        <td>
          <code>--bs-danger-bg-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="border: 5px var(--bs-danger-border-subtle) solid">&nbsp;</div>
        </td>
        <td>
          <code>--bs-danger-border-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="py-3 fw-bold h5" style="color: var(--bs-danger-text-emphasis)">Text</div>
        </td>
        <td>
          <code>--bs-danger-text-emphasis</code>
        </td>
      </tr>
      <tr>
        <td rowspan="4" class="align-top"><strong>Warning —</strong> Theme color used for non-destructive warning messages.</td>
        <td>
          <div class="p-3 rounded-2 bg-warning">&nbsp;</div>
        </td>
        <td><code>--bs-warning</code><br /><code>--bs-warning-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-warning-bg-subtle)">&nbsp;</div>
        </td>
        <td>
          <code>--bs-warning-bg-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="border: 5px var(--bs-warning-border-subtle) solid">&nbsp;</div>
        </td>
        <td>
          <code>--bs-warning-border-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="py-3 fw-bold h5" style="color: var(--bs-warning-text-emphasis)">Text</div>
        </td>
        <td>
          <code>--bs-warning-text-emphasis</code>
        </td>
      </tr>
      <tr>
        <td rowspan="4" class="align-top"><strong>Info —</strong> Theme color used for neutral and informative content.</td>
        <td>
          <div class="p-3 rounded-2 bg-info">&nbsp;</div>
        </td>
        <td><code>--bs-info</code><br /><code>--bs-info-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-info-bg-subtle)">&nbsp;</div>
        </td>
        <td>
          <code>--bs-info-bg-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="border: 5px var(--bs-info-border-subtle) solid">&nbsp;</div>
        </td>
        <td>
          <code>--bs-info-border-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="py-3 fw-bold h5" style="color: var(--bs-info-text-emphasis)">Text</div>
        </td>
        <td>
          <code>--bs-info-text-emphasis</code>
        </td>
      </tr>
      <tr>
        <td rowspan="4" class="align-top"><strong>Light —</strong> Additional theme option for less contrasting colors.</td>
        <td>
          <div class="p-3 rounded-2 bg-light">&nbsp;</div>
        </td>
        <td><code>--bs-light</code><br /><code>--bs-light-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-light-bg-subtle)">&nbsp;</div>
        </td>
        <td>
          <code>--bs-light-bg-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="border: 5px var(--bs-light-border-subtle) solid">&nbsp;</div>
        </td>
        <td>
          <code>--bs-light-border-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="py-3 fw-bold h5" style="color: var(--bs-light-text-emphasis)">Text</div>
        </td>
        <td>
          <code>--bs-light-text-emphasis</code>
        </td>
      </tr>
      <tr>
        <td rowspan="4" class="align-top"><strong>Dark —</strong> Additional theme option for higher contrasting colors.</td>
        <td>
          <div class="p-3 rounded-2 bg-dark">&nbsp;</div>
        </td>
        <td><code>--bs-dark</code><br /><code>--bs-dark-rgb</code></td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="background-color: var(--bs-dark-bg-subtle)">&nbsp;</div>
        </td>
        <td>
          <code>--bs-dark-bg-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="p-3 rounded-2" style="border: 5px var(--bs-dark-border-subtle) solid">&nbsp;</div>
        </td>
        <td>
          <code>--bs-dark-border-subtle</code>
        </td>
      </tr>
      <tr>
        <td>
          <div class="py-3 fw-bold h5" style="color: var(--bs-dark-text-emphasis)">Text</div>
        </td>
        <td>
          <code>--bs-dark-text-emphasis</code>
        </td>
      </tr>
    </tbody>
  </table>
</div>


## Color palette

{{< palette.inline >}}
<div class="row g-3 mt-4">
  {{ range .Site.Data.colors }}
    {{ range $title, $colors := . }}
      {{ if not (in (slice "Neutral" "DarkNeutral") $title) }}
        <div class="col-md-6 col-lg-4">
          <p class="fw-bold fs-sm">{{ $title }}</p>
          <ul class="list-unstyled">
            {{ range $colors }}
              {{ range $depth, $color := . }}
                {{ $name := printf "%s%s" $title $depth }}
                {{ $text := "black"}}
                <li class="py-2 ps-4 pe-2 bd-h-9 w-100 d-inline-flex align-items-center" style="background: {{ $color }}">
                  <div class="fs-sm" style="color:{{ if lt $depth 700 }}black{{ else }}white{{ end }}">{{ $name }}</div>
                </li>
              {{ end }}
            {{ end }}
          </ul>
        </div>   
      {{ end }}      
    {{ end }}  
  {{ end }} 
</div>

{{ range .Site.Data.colors }}
  {{ range $title, $values := . }}
    {{ if (in (slice "Neutral" "DarkNeutral") $title) }}
      {{ $dark := eq $title "DarkNeutral" }}
      <h3 class="mt-4">{{ cond $dark "Dark mode neutrals" "Light mode neutrals" }}</h3>
       <div class="row g-3 mt-2 rounded" style="background-color:{{ cond $dark "#161A1D" "#FAFBFC" }}">
        {{ range $values }}
          {{ range $style, $colors := .}}
            <div class="col-md-6">
            <p class="fw-bold fs-sm" style="color:{{if $dark}}#C7D1DB{{end}}">{{ $style }}</p>
            <ul class="list-unstyled">
              {{ range $colors }}                  
                {{ range $depth, $color := . }}
                  {{ $name := printf "%s%s" $title $depth }}
                  {{ $text := "black"}}
                  <li class="py-2 ps-4 pe-2 bd-h-9 w-100 d-inline-flex align-items-center" style="background: {{ $color }}">
                    {{- $isWhite := false -}}
                    {{- if and $dark (le $depth 500 ) -}}
                      {{- $isWhite = true -}}
                    {{- else if and (ne $dark true) (ge $depth 700 ) -}}
                      {{- $isWhite = true -}}
                    {{ end }}
                    <div class="fs-sm" style="color:{{ cond $isWhite "white" "black" }}">{{ $name }}</div>
                  </li>
                {{ end }}
              {{ end }}
            </ul>
            </div>
          {{ end }}
        {{ end }}
        </div>
    {{ end }}
  {{ end }}
{{ end}}

{{</ palette.inline >}}