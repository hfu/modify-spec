# modify-spec
## use
```node
const modify = require('modify-some-data')
/// ...
  json = modify(json)
  if(json) console.log(json)
/// ...
```

## define
```node
// this is modify-some-data.js
module.exports = function(f) {
  f.tippecanoe = {minzoom: 2, maxzoom: 5, layer: 'some'}
  return f
}
```

## specifications
### If the feature shall be deleted, the modify function shall return false.
### Otherwise, the modify function shall return the modified object.

## actual use of this specifications
FIXME
