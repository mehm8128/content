---
title: Map.prototype.has()
short-title: has()
slug: Web/JavaScript/Reference/Global_Objects/Map/has
page-type: javascript-instance-method
browser-compat: javascript.builtins.Map.has
sidebar: jsref
---

The **`has()`** method of {{jsxref("Map")}} instances returns a boolean indicating whether an element with the
specified key exists in this map or not.

{{InteractiveExample("JavaScript Demo: Map.prototype.has()")}}

```js interactive-example
const map = new Map();
map.set("bar", "foo");

console.log(map.has("bar"));
// Expected output: true

console.log(map.has("baz"));
// Expected output: false
```

## Syntax

```js-nolint
has(key)
```

### Parameters

- `key`
  - : The key of the element to test for presence in the `Map` object.

### Return value

`true` if an element with the specified key exists in the `Map` object;
otherwise `false`.

## Examples

### Using has()

```js
const myMap = new Map();
myMap.set("bar", "foo");

console.log(myMap.has("bar")); // true
console.log(myMap.has("baz")); // false
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{jsxref("Map")}}
- {{jsxref("Map.prototype.set()")}}
- {{jsxref("Map.prototype.get()")}}
