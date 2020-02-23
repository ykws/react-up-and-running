# Book's differents

## 1.2

```diff
-<script src="react/build/react.js"></script>
-<script src="react/build/react-dom.js"></script>
+<script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
+<script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
```

```diff
- React.DOM.h1(hull, "Hello, world!"),
+ React.createElement('h1', null, 'Hello, world!'),
```

## References
* [CDN Links](https://reactjs.org/docs/cdn-links.html)
* [React Without JSX](https://reactjs.org/docs/react-without-jsx.html)
* [React Top-Level API - React createElement()](https://reactjs.org/docs/react-api.html#createelement)

