[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/value-history)

# value-history
Record property changes with this handy little element.

## Installation

```
bower install --save value-history
```

## Usage
Primarily for use with `app-location` in client-side routed apps, or
for debugging and testing.
* Tell it which property to watch for changes
* Optionally limit the history to a certain length.

## Demo
<!--
```
<custom-element-demo>
  <dom-bind>
  <template is="dom-bind">
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="value-history.html">
    <next-code-block></next-code-block>
  </template>
  </dom-bind>
</custom-element-demo>
```
-->

```html
<value-history value="[[val]]" history="{{history}}" limit="[[limit]]"></value-history>
<input placeholder="value" value="{{val::input}}" length="5"/><br/>
<input placeholder="limit" value="{{limit::input}}" length="5"/>
<dom-repeat items="[[history]]">
  <template>[[item]]<br/></template>
</dom-repeat>
<i style="font-size: small">Polymer bindings may not work in this readme demo.</i>
```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/value-history/demo/demo/index.html)
| [github](https://jifalops.github.io/value-history/components/value-history/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/value-history/value-history)


## Releases
Version | Description
------- | -----------
0.2.0 | Polymer 1.x and 2.0 compatible (hybrid mode)
0.1.0 | Polymer 1.x based

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
