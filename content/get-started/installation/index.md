---
layout: docs
title: Installation
description: "Download the compiled CSS and JS, all source code."
toc: true
icon: fa-solid fa-cube
menu:
  get-started:
weight: 10
---

Download FastBootstrap to get the compiled CSS and JavaScript, source code, or include it with your favorite package managers like npm and more.

## Compiled CSS and JS

Download ready-to-use compiled code for **FastBootstrap v{{< param "current_version" >}}** to easily drop into your project, which includes:

- Compiled and minified CSS bundles
- <del>Compiled and minified JavaScript plugins</del>

<a class="btn btn-primary btn-lg" href="{{< param "download.source" >}}">Download</a>

## CDN via jsDelivr

We recommend using [jsDelivr](https://www.jsdelivr.com/) to deliver cached version of FastBootstrap’s compiled CSS and JS to your project.

### CSS file

Place this tag in your head.

```html
<link href="{{< param "cdn.css">}}" rel="stylesheet" integrity="{{< param "cdn.css_hash">}}" crossorigin="anonymous">
```

### JS file

Place this tag in your head or just before your close body tag.

```html
<script src="{{< param "bootstrap.cdn.js_bundle" >}}" integrity="{{< param "bootstrap.cdn.js_bundle_hash" >}}" crossorigin="anonymous"></script>
```

## Source files

All source code files are on [github](https://github.com/fastbootstrap/atlassian-design-for-bootstrap). 


## Package managers 

### npm  

Install with the npm package:

```bash 
npm install fastbootstrap
```

## What to read next

- [Start your project with FastBootstrap in minute]({{< docsref "quick-start" >}})
- [How to enable dark mode]({{< docsref "dark-mode" >}})
