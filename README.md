# Web Icons

An investigation into the future of icons on the Web.

## Overview

Traditionally, the web has been full of raster graphics, such as `.jpg`, `.png`, and `.gif` files. These have been used because they had the best browser support. However, all raster graphics have several drawbacks, which we will attempt to outline in detail. Many sites are now using vector graphics for icons to overcome some of the limitations inherit in raster graphics. Two major replacements have been SVG images and icon fonts. However, neither of these are ideal solutions. This project is an attempt to outline, in detail, all of the pros and cons of every option that is available today. The goal is to find, or create, the ideal implementation for icons on the Web.

## Goals

### Broad browser support

In order for any solution to be acceptable, it must have extremely broad support. The following browsers are the minimum requirement:

* IE 8+
* Chrome stable
* Firefox stable
* Safari 5+
* Opera 12+

### Scalable to any size

Icons should scale cleanly. Scaling is important for several reasons:

* HiDPI screens are becoming more and more common.
* Users may zoom the page, causing the image to scale.
* Icons will be used at varying sizes on different web sites.

### Pixel perfect at small sizes

One drawback to vector graphics is that as the image is scaled down, the quality may decrease. Traditional desktop icons combat this problem by manually adjusting the images at common sizes. Web icons should have the same ability.

### Accessible

Icons must be easy to use in an accessible manner. Sometimes icons will need a textual representation and sometimes they won't.

### Display in any color

Traditional icons are rendered in a specific, pre-defined, color. Icons should support dynamically setting the color, especially by inheriting the current text color.

### Multi-colored icons

Icons should be able to render in multiple colors. Rendering a logo in its original colors should use the same markup as rendering a single-colored icon that inherits from the current font color.

### Support for dynamic content

Icons need to "just work". The API for using an icon should not include anything but writing some simple markup.

### Animated/interactive icons

Animation is a nice-to-have feature, and should be used sparingly.
