---
title: "FormData: keys() method"
short-title: keys()
slug: Web/API/FormData/keys
page-type: web-api-instance-method
browser-compat: api.FormData.keys
---

{{APIRef("XMLHttpRequest API")}}

The **`FormData.keys()`** method returns an [iterator](/en-US/docs/Web/JavaScript/Reference/Iteration_protocols) which iterates through all keys contained in the {{domxref("FormData")}}. The keys are strings.

> **Note:** This method is available in [Web Workers](/en-US/docs/Web/API/Web_Workers_API).

## Syntax

```js-nolint
keys()
```

### Parameters

None.

### Return value

An [`iterator`](/en-US/docs/Web/JavaScript/Reference/Iteration_protocols) of {{domxref("FormData")}}'s keys.

## Examples

```js
const formData = new FormData();
formData.append("key1", "value1");
formData.append("key2", "value2");

// Display the keys
for (const key of formData.keys()) {
  console.log(key);
}
```

The result is:

```plain
key1
key2
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Using FormData objects](/en-US/docs/Web/API/XMLHttpRequest_API/Using_FormData_Objects)
- {{HTMLElement("Form")}}
