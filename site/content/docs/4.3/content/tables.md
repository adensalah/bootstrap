---
layout: docs
title: Tables
description: Documentation and examples for opt-in styling of tables (given their prevalent use in JavaScript plugins) with Bootstrap.
group: content
toc: true
---

## Overview

Due to the widespread use of `<table>` elements across third-party widgets like calendars and date pickers, Bootstrap's tables are **opt-in**. Add the base class `.table` to any `<table>`, then extend with our optional modifier classes or custom styles. **All table styles are inherited in Bootstrap**, meaning any nested tables will be styled in the same manner as the parent.

Using the most basic table markup, here's how `.table`-based tables look in Bootstrap.

{{< example >}}
<table class="table">
{{< partial "table-content.html" ->}}</table>
{{< /example >}}

## Options

### Inverted

You can also invert the colors—with light text on dark backgrounds—with `.table-dark`.

<div class="bd-example">
  <table class="table table-dark">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-dark">
  ...
</table>
{{< /highlight >}}

### Striped rows

Use `.table-striped` to add zebra-striping to any table row within the `<tbody>`.

<div class="bd-example">
  <table class="table table-striped">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-striped">
  ...
</table>
{{< /highlight >}}

<div class="bd-example">
  <table class="table table-striped table-dark">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-striped table-dark">
  ...
</table>
{{< /highlight >}}

### Bordered

Add `.table-bordered` for borders on all sides of the table and cells.

<div class="bd-example">
  <table class="table table-bordered">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-bordered">
  ...
</table>
{{< /highlight >}}

[Border color utilities]({{< docsref "/utilities/borders#border-color" >}}) can be added to change colors:

<div class="bd-example">
  <table class="table table-bordered border-primary">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-bordered border-primary">
  ...
</table>
{{< /highlight >}}

<div class="bd-example">
  <table class="table table-bordered table-dark">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-bordered table-dark">
  ...
</table>
{{< /highlight >}}

### No borders

Add `.table-borderless` for a table without borders.

<div class="bd-example">
  <table class="table table-borderless">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-borderless">
  ...
</table>
{{< /highlight >}}

<div class="bd-example">
  <table class="table table-borderless table-dark">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-borderless table-dark">
  ...
</table>
{{< /highlight >}}

### Hoverable rows

Add `.table-hover` to enable a hover state on table rows within a `<tbody>`.

<div class="bd-example">
  <table class="table table-hover">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-hover">
  ...
</table>
{{< /highlight >}}

<div class="bd-example">
  <table class="table table-hover table-dark">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-hover table-dark">
  ...
</table>
{{< /highlight >}}

### Small tables

Add `.table-sm` to make any `.table` more compact by cutting all cell `padding` in half.

<div class="bd-example">
  <table class="table table-sm">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-sm">
  ...
</table>
{{< /highlight >}}

<div class="bd-example">
  <table class="table table-sm table-dark">
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-sm table-dark">
  ...
</table>
{{< /highlight >}}

## Vertical alignment

Table cells of `<thead>` are always vertical aligned to the bottom. Table cells in `<tbody>` inherit their alignment from `<table>` and are aligned to the the top by default.

<div class="bd-example">
  <div class="table-responsive">
    <table class="table align-middle">
      <thead>
        <tr>
          <th scope="col" class="w-25">Heading 1</th>
          <th scope="col" class="w-25">Heading 2</th>
          <th scope="col" class="w-25">Heading 2</th>
          <th scope="col" class="w-25">Heading 4</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>This cell inherits <code>vertical-align: middle;</code> from the table</td>
          <td>This cell inherits <code>vertical-align: middle;</code> from the table</td>
          <td>This cell inherits <code>vertical-align: middle;</code> from the table</td>
          <td>Nulla vitae elit libero, a pharetra augue. Cras mattis consectetur purus sit amet fermentum. Vestibulum id ligula porta felis euismod semper.</td>
        </tr>
        <tr class="align-bottom">
          <td>This cell inherits <code>vertical-align: bottom;</code> from the table row</td>
          <td>This cell inherits <code>vertical-align: bottom;</code> from the table row</td>
          <td>This cell inherits <code>vertical-align: bottom;</code> from the table row</td>
          <td>Nulla vitae elit libero, a pharetra augue. Cras mattis consectetur purus sit amet fermentum. Vestibulum id ligula porta felis euismod semper.</td>
        </tr>
        <tr>
          <td>This cell inherits <code>vertical-align: middle;</code> from the table</td>
          <td>This cell inherits <code>vertical-align: middle;</code> from the table</td>
          <td class="align-top">This cell is aligned to the top.</td>
          <td>Nulla vitae elit libero, a pharetra augue. Cras mattis consectetur purus sit amet fermentum. Vestibulum id ligula porta felis euismod semper.</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

{{< highlight html >}}
<table class="table table-sm table-dark">
  <div class="table-responsive">
    <table class="table align-middle">
      <thead>
        <tr>
          ...
        </tr>
      </thead>
      <tbody>
        <tr>
          ...
        </tr>
        <tr class="align-bottom">
          ...
        </tr>
        <tr>
          <td>...</td>
          <td>...</td>
          <td class="align-top">This cell is aligned to the top.</td>
          <td>...</td>
        </tr>
      </tbody>
    </table>
  </div>
</table>
{{< /highlight >}}

## Variants

Use contextual classes to color table rows or individual cells.

<div class="bd-example">
  <table class="table">
    <thead>
      <tr>
        <th scope="col">Class</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
      </tr>
    </thead>
    <tbody>
      <tr class="table-active">
        <th scope="row">Active</th>
        <td>Cell</td>
        <td>Cell</td>
      </tr>
      <tr>
        <th scope="row">Default</th>
        <td>Cell</td>
        <td>Cell</td>
      </tr>
      {{< table.inline >}}
      {{- range (index $.Site.Data "theme-colors") }}
        <tr class="table-{{ .name }}">
          <th scope="row">{{ .name | title }}</th>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
      {{- end -}}
      {{< /table.inline >}}
    </tbody>
  </table>
</div>

{{< highlight html >}}
<!-- On rows -->
<tr class="table-active">...</tr>{{< table.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<tr class="table-{{ .name }}">...</tr>
{{- end -}}
{{< /table.inline >}}

<!-- On cells (`td` or `th`) -->
<tr>
  <td class="table-active">...</td>{{< table.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
  <td class="table-{{ .name }}">...</td>
{{- end -}}
{{< /table.inline >}}
</tr>
{{< /highlight >}}

{{< callout info >}}
{{< partial "callout-warning-color-assistive-technologies.md" >}}
{{< /callout >}}

## Anatomy

### Table head

Similar to tables and dark tables, use the modifier classes `.thead-light` or `.thead-dark` to make `<thead>`s appear light or dark gray.

<div class="bd-example">
<table class="table">
  <thead class="table-light">
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Larry</td>
      <td>the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
</div>

{{< highlight html >}}
<table class="table">
  <thead class="table-light">
    ...
  </thead>
  <tbody>
    ...
  </tbody>
</table>
{{< /highlight >}}

<div class="bd-example">
<table class="table">
  <thead class="table-dark">
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Larry</td>
      <td>the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
</div>

{{< highlight html >}}
<table class="table">
  <thead class="table-dark">
    ...
  </thead>
  <tbody>
    ...
  </tbody>
</table>
{{< /highlight >}}

### Captions

A `<caption>` functions like a heading for a table. It helps users with screen readers to find a table and understand what it's about and decide if they want to read it.

<div class="bd-example">
  <table class="table">
    <caption>List of users</caption>
    {{< partial "table-content.html" >}}
  </table>
</div>

{{< highlight html >}}
<table class="table table-sm">
  <caption>List of users</caption>
  <thead>
    ...
  </thead>
  <tbody>
    ...
  </tbody>
</table>
{{< /highlight >}}

You can also put the `<caption>` on the top of the table with `.caption-top`.

{{< example >}}
<table class="table caption-top">
  <caption>List of users</caption>
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Larry</td>
      <td>the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
{{< /example >}}

## Responsive tables

Responsive tables allow tables to be scrolled horizontally with ease. Make any table responsive across all viewports by wrapping a `.table` with `.table-responsive`. Or, pick a maximum breakpoint with which to have a responsive table up to by using `.table-responsive{-sm|-md|-lg|-xl}`.

{{< callout warning >}}
##### Vertical clipping/truncation

Responsive tables make use of `overflow-y: hidden`, which clips off any content that goes beyond the bottom or top edges of the table. In particular, this can clip off dropdown menus and other third-party widgets.
{{< /callout >}}

### Always responsive

Across every breakpoint, use `.table-responsive` for horizontally scrolling tables.

<div class="bd-example">
  <div class="table-responsive">
    <table class="table">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
        <tr>
          <th scope="row">2</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
        <tr>
          <th scope="row">3</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

{{< highlight html >}}
<div class="table-responsive">
  <table class="table">
    ...
  </table>
</div>
{{< /highlight >}}

### Breakpoint specific

Use `.table-responsive{-sm|-md|-lg|-xl}` as needed to create responsive tables up to a particular breakpoint. From that breakpoint and up, the table will behave normally and not scroll horizontally.

**These tables may appear broken until their responsive styles apply at specific viewport widths.**

{{< tables.inline >}}
{{ range $.Site.Data.breakpoints }}
{{ if not (eq . "xs") }}
<div class="bd-example">
  <div class="table-responsive{{ .abbr }}">
    <table class="table">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
          <th scope="col">Heading</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
        <tr>
          <th scope="row">2</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
        <tr>
          <th scope="row">3</th>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
          <td>Cell</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
{{ end -}}
{{- end -}}
{{< /tables.inline >}}

{{< highlight html >}}
{{< tables.inline >}}
{{- range $.Site.Data.breakpoints -}}
{{- if not (eq . "xs") }}
<div class="table-responsive{{ .abbr }}">
  <table class="table">
    ...
  </table>
</div>
{{ end -}}
{{- end -}}
{{< /tables.inline >}}
{{< /highlight >}}
