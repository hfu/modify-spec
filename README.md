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
// modify.js
module.exports = f => {
  f.tippecanoe = {minzoom: 2, maxzoom: 5, layer: 'some'}
  return f
}
```

## specifications
1. If the feature shall be deleted, the modify function shall return false.
2. Otherwise, the modify function shall return the modified object.

## actual use of this specifications
### os-gpkg-vt
[modify.js](https://github.com/hfu/os-gpkg-vt/blob/master/modify.js) works for [index.js](https://github.com/hfu/os-gpkg-vt/blob/master/index.js).

### pnd
[pnd](https://github.com/hfu/pnd/) was renovated to use modify-spec. 
