---
title: "EncodedAudioChunk: timestamp property"
short-title: timestamp
slug: Web/API/EncodedAudioChunk/timestamp
page-type: web-api-instance-property
browser-compat: api.EncodedAudioChunk.timestamp
---

{{APIRef("WebCodecs API")}}{{AvailableInWorkers("window_and_dedicated")}}

The **`timestamp`** read-only property of the {{domxref("EncodedAudioChunk")}} interface returns an integer indicating the timestamp of the audio in microseconds.

## Value

An integer.

## Examples

In the following example the `timestamp` is printed to the console.

```js
const init = {
  type: "key",
  data: audioBuffer,
  timestamp: 23000000,
  duration: 2000000,
};
const chunk = new EncodedAudioChunk(init);

console.log(chunk.timestamp); // 23000000
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
