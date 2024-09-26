# osm-adiff-parser-saxjs

Parses OSM augmented diff (`.adiff`) files and returns elements grouped by changeset ids.

> [!WARNING]
> This package is deprecated. Instead, use [`@osmcha/osm-adiff-parser`](https://www.npmjs.com/package/@osmcha/osm-adiff-parser) v2.0.0 or higher, which works both in Node.js and in browsers.

## Setup

* npm install --save osm-adiff-parser

## Usage

```js

var parser = require('osm-adiff-parser');

// to filter certain changesets

parser(xml, ['46613588', '46613589'], function(err,data) {
    console.log(data);
});

// to get all changesets

parser(xml, null, function(err,data) {
    console.log(data);
});

```
