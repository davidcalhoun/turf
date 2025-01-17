# @turf/rectangle-grid

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## rectangleGrid

Creates a grid of rectangles from a bounding box, [Feature][1] or [FeatureCollection][2].

### Parameters

*   `bbox` **[Array][3]<[number][4]>** extent in \[minX, minY, maxX, maxY] order
*   `cellWidth` **[number][4]** of each cell, in units
*   `cellHeight` **[number][4]** of each cell, in units
*   `options` **[Object][5]** Optional parameters (optional, default `{}`)

    *   `options.units` **[string][6]** units ("degrees", "radians", "miles", "kilometers") that the given cellWidth
        and cellHeight are expressed in. Converted at the southern border. (optional, default `'kilometers'`)
    *   `options.mask` **[Feature][7]<([Polygon][8] | [MultiPolygon][9])>?** if passed a Polygon or MultiPolygon,
        the grid Points will be created only inside it
    *   `options.properties` **[Object][5]** passed to each point of the grid (optional, default `{}`)

### Examples

```javascript
var bbox = [-95, 30 ,-85, 40];
var cellWidth = 50;
var cellHeight = 20;
var options = {units: 'miles'};

var rectangleGrid = turf.rectangleGrid(bbox, cellWidth, cellHeight, options);

//addToMap
var addToMap = [rectangleGrid]
```

Returns **[FeatureCollection][10]<[Polygon][8]>** a grid of polygons

[1]: https://tools.ietf.org/html/rfc7946#section-3.2

[2]: https://tools.ietf.org/html/rfc7946#section-3.3

[3]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array

[4]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

[5]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[6]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[7]: https://tools.ietf.org/html/rfc7946#section-3.2

[8]: https://tools.ietf.org/html/rfc7946#section-3.1.6

[9]: https://tools.ietf.org/html/rfc7946#section-3.1.7

[10]: https://tools.ietf.org/html/rfc7946#section-3.3

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/rectangle-grid
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
