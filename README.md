# bify-packagedata-stream

A browserify utility to append additional package data to module objects.
Useful for browserify plugin authors.

### use

```js
const { createPackageDataStream } = require('bify-packagedata-stream')

// inject package name into module data
browserify.pipeline.get('emit-deps').unshift(createPackageDataStream())
```