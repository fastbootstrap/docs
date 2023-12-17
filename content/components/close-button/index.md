---
layout: docs
title: Close Button
description: "A close button used for dismissing content like modals and alerts."
toc: true
group: actions
menu:
  components:
---

**Bootstrap 5 Close button component**

Close button built with the latest Bootstrap 5. The close button component is used for dismissing content like modals and alerts.

## Close button

Provide an option to dismiss or close a component with `.btn-close`. Default styling is limited, but highly customizable. Modify the Sass variables to replace the default `background-image`. Be sure to include text for screen readers by `aria-label`.

{{< example >}}
<button type="button" class="btn-close" aria-label="Close"></button>
{{</ example >}}

## Disabled state

You can disable a close button by adding the `disabled` attribute. We’ve also applied `pointer-events: none` and `user-select: none` to prevent hover and active states from being triggered.

{{< example >}}
<button type="button" class="btn-close" disabled aria-label="Close"></button>
{{</ example >}}

## Sizes

<span class="lozenge new fs-sm">New Feature</span>

Use the `.btn-close-sm` for the smaller close button.

{{< example >}}
<button type="button" class="btn-close btn-close-sm" aria-label="Close"></button>
{{</ example >}}

Or set the `--bs-btn-close-width` and `--bs-btn-close-height` CSS variables to desired values for custom sizing.

{{< example >}}
<button type="button" class="btn-close" aria-label="Close"
 style="
 --bs-btn-close-width:32px;
 --bs-btn-close-height:32px">
</button>
{{</ example >}}