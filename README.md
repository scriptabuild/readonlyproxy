# readonlyproxy

Creates a wrapper that looks like the object it wraps, but only provides read only access.

```bash
npm install @scriptabuild/readonlyproxy
```

Example usage:
```javascript
const wrapInReadOnlyProxy = require("@scriptabuild/readonlyproxy");

let originalObject = { /* lots of properties and nested properties */ };
let wrappedObject = wrapInReadOnlyProxy(originalObject);

// Its not possible to change value on any propery via wrappedObject.
// If you change a property on originalObject, that change is
// immediatly visible through wrappedObject.
```