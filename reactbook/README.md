# Book's differences

## 1.2

```diff
-<script src="react/build/react.js"></script>
-<script src="react/build/react-dom.js"></script>
+<script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
+<script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
```

```diff
- React.DOM.h1(null, "Hello, world!"),
+ React.createElement('h1', null, 'Hello, world!'),
```


```diff
- React.DOM.h1(
+ React.createElement('h1',
    {id: "my-heading"},
-   React.DOM.span(null, "Hell"),
+   React.createElement('span', null, "Hell"),
    " world!"
```

```diff
- React.DOM.h1(
+ React.createElement('h1',
    {id: "my-heading"},
-   React.DOM.span(null,
+   React.createElement('span', null
-     React.DOM.em(null, "Hell"),
+     React.createElement('em', null, "Hell"),
      "o"
    ),
    " world!"
```

## 2.1

```diff
- var MyComponent = React.createClass({
+ class MyComponent extends React.Component {
```

```diff
- var Component = React.createClass({
-   render: function() {
-     return React.DOM.span(null, "カスタムコンポーネント");
+ class Component extends React.Component {
+   render() { 
+     return React.createElement('span', null, "カスタムコンポーネント");
```

## 2.3

```diff
- var Component = React.createClass({
-   propTypes: {
-     name: React.PropTypes.string.isRequired,
-   },
-   render: function() {
-     return React.DOM.span(null, "カスタムコンポーネント");
+ class Component extends React.Component {
+   render() { 
+     return React.createElement('span', null, "カスタムコンポーネント");
    }
  }
+ Component.propTypes = {
+   name: PropTypes.string.isRequired,
+ };
```

```diff
- Object.keys(React.PropTypes)
+ Object.keys(PropTypes)
```

## References
* [CDN Links](https://reactjs.org/docs/cdn-links.html)
* [React Without JSX](https://reactjs.org/docs/react-without-jsx.html)
* [React Top-Level API - React createElement()](https://reactjs.org/docs/react-api.html#createelement)
* [Components and Props](https://reactjs.org/docs/components-and-props.html)
* [Typechecking With PropTypes](https://reactjs.org/docs/typechecking-with-proptypes.html)
* [prop-types](https://github.com/facebook/prop-types)
