
# escape-html

  Escape string for use in HTML

## Example

```js
var escape = require('escape-html');
var html = escape('foo & bar');
// -> foo &amp; bar
```

## Benchmark

```
$ npm run-script bench

> escape-html@1.0.3-pre bench nodejs-escape-html
> node benchmark/index.js


  http_parser@1.0
  node@0.10.33
  v8@3.14.5.9
  ares@1.9.0-DEV
  uv@0.10.29
  zlib@1.2.3
  modules@11
  openssl@1.0.1j

  1 test completed.
  2 tests completed.
  3 tests completed.

  no special characters    x 15,913,255 ops/sec ±1.10% (187 runs sampled)
  single special character x  5,610,789 ops/sec ±0.84% (192 runs sampled)
  many special characters  x  3,042,399 ops/sec ±1.04% (193 runs sampled)
```

## License

  MIT