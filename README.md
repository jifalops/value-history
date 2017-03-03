[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/value-history)

# value-history
Record property changes with this handy little element.

## Installation

```
bower install --save value-history
```

## Usage
* Tell it which property to watch for changes
* Optionally limit the history to a certain length.

## Demo
<!--
```
<custom-element-demo>
  <template is="dom-bind">
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>    
    <link rel="import" href="value-history.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->

```html
<value-history
  value="[[someObj]]"
  history="{{history}}"
  limit="[[limit]]">
</value-history>
<input placeholder="value" value="{{someObj::input}}" length="5"/><br/>
<input placeholder="limit" value="{{limit::input}}" length="5"/>
<template is="dom-repeat" items="[[history]]">
  <div>[[item]]</div>
</template>

```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/value-history/demo/demo/index.html)
| [github](https://jifalops.github.io/value-history/components/value-history/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/value-history/value-history)
| [github](https://jifalops.github.io/value-history).


## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
