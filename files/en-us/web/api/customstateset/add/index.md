---
title: "CustomStateSet: add() method"
short-title: add()
slug: Web/API/CustomStateSet/add
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.CustomStateSet.add
---

{{APIRef("Web Components")}}{{SeeCompatTable}}

The **`add`** method of the {{domxref("CustomStateSet")}} interface adds an item to the `CustomStateSet`, after checking that the value is in the correct format.

## Syntax

```js-nolint
add(value)
```

### Parameters

- `value`
  - : A string which must be a `<dashed-ident>`, with the form `--mystate`.

### Return value

Undefined.

### Exceptions

- `SyntaxError` {{domxref("DOMException")}}
  - : Thrown if the string is not a `<dashed-ident>`.

## Examples

The following function adds the state `--checked` to a `CustomStateSet`.

```js
class MyCustomElement extends HTMLElement {
  set checked(flag) {
    if (flag) {
      this._internals.states.add("--checked");
    }
  }
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
