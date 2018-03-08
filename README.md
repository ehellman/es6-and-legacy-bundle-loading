# es6-and-legacy-bundle-loading

Give `window.__APP_CHUNKS__` the paths to your ES6 and legacy bundles/chunks and the script will load the correct bundle by checking if the browser supports `<script type="module">`.

```
window.__APP_CHUNKS__ = {
  es: [
    '/main.js',
    '/first.chunk.js',
    '/second.chunk.js'
  ],
  legacy: [
    '/main.legacy.js',
    '/first.legacy.chunk.js',
    '/second.legacy.chunk.js'
  ]
};
```