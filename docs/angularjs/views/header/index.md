---
layout: docs_0.9.0
active: angularjs
title: "Headers"
header_sub_title: "Headers"
---

Available in:
<div class="label label-danger">Ionic-Angular 0.9.0</div>
<div class="label label-primary">Ionic 0.9.0</div>


Headers
===

While Ionic provides [simple Header and Footer](/docs/components/#header) bars that can be created through HTML and CSS alone, Header bars specifically can be extended in order to provide dynamic layout features such as auto-title centering and animation. They are also used by the [Nav Router Controller](../../controllers/nav-router/) to animate a title on navigation and toggle a back button.

As of Ionic 0.9.0, the only available header bar feature provide is auto title centering. In this situation, the title text will center itself until either the left or right button content is too wide for the label to center. In that case, it will slide left or right until it can fit. You can also align the title left for a more Android-friendly header.

Using two-way data binding, the header bar will automatically readjust the heading title alignment when the title or buttons change.

## Ionic-Angular Usage

To use the dynamic header bar behavior in Ionic-Angular, use the `<header-bar>` directive:

```html
<header-bar
  title="headerTitle"
  left-buttons="leftButtons"
  right-buttons="rightButtons"
  type="bar-primary"
  align-title="center">
</header-bar>

```

Where `headerTitle`, `leftButtons`, and `rightButtons` are angular expressions. Pass in `left` for the `align-title` attribute to align the title to the left for more Android-friendly layouts.