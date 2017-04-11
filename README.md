# build-and-run-aggregation

A Polymer Element that builds and runs an elasticsearch aggregation query and returns the transformed results.

### Example
```html
<build-and-run-aggregation
  aggregation-field="myAggregationField"
  fields='"myField"'
  values='"myValue"'
  client="[[client]]"
  index-name="myIndexName"
  index-types='["myIndexType"]'
  transform-function="[[myFunction]]"
  error="{{error}}"
  loading="{{loading}}"
  results="{{results}}">
</build-and-run-aggregation>
```

### Raw Elasticsearch Results

To return the raw elasticsearch results rather than the results of the transform function, set the "raw" property.

```html
<build-and-run-aggregation
  raw
  aggregation-field="myAggregationField"
  fields='"myField"'
  values='"myValue"'
  client="[[client]]"
  index-name="myIndexName"
  index-types='["myIndexType"]'
  error="{{error}}"
  loading="{{loading}}"
  results="{{results}}">
</build-and-run-aggregation>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

