# modify-spec
## use
```node
const modify = require('./modify.js')
/// ...
  f = modify(f)
  if (f) console.log(f)
/// ...
```

## define
```node
// this is modify.js
module.exports = (f) => {
  f.tippecanoe = {minzoom: 2, maxzoom: 5, layer: 'some'}
  return f
}
```

## specifications
### If the feature shall be deleted, the modify function shall return false.
### Otherwise, the modify function shall return the modified object.

## actual use of this specifications
### os-gpkg-vt
[modify.js](https://github.com/hfu/os-gpkg-vt/blob/master/modify.js) works for [index.js](https://github.com/hfu/os-gpkg-vt/blob/master/index.js).
