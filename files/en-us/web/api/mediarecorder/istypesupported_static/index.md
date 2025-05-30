---
title: "MediaRecorder: isTypeSupported() static method"
short-title: isTypeSupported()
slug: Web/API/MediaRecorder/isTypeSupported_static
page-type: web-api-static-method
browser-compat: api.MediaRecorder.isTypeSupported_static
---

{{APIRef("MediaStream Recording")}}

The **`isTypeSupported()`** static method of the {{domxref("MediaRecorder")}} interface returns a {{jsxref("Boolean")}} which is `true` if the MIME media type specified is one the user agent should be able to successfully record.

## Syntax

```js-nolint
MediaRecorder.isTypeSupported(mimeType)
```

### Parameters

- `mimeType`
  - : The MIME media type to check.

### Return value

A {{jsxref("Boolean")}}, `true` if the {{domxref("MediaRecorder")}} implementation is capable of recording {{domxref("Blob")}} objects for the specified MIME type.
Recording may still fail if there are insufficient resources to support the recording and encoding process.
If the value is `false`, the user agent is incapable of recording the specified format.

## Examples

```js
const types = [
  "video/webm",
  "audio/webm",
  "video/webm;codecs=vp8",
  "video/webm;codecs=daala",
  "video/webm;codecs=h264",
  "audio/webm;codecs=opus",
  "video/mp4",
  "video/mp4;codecs=avc1.64003E,mp4a.40.2",
  "video/mp4;codecs=avc1.64003E,opus",
  "video/mp4;codecs=avc3.64003E,mp4a.40.2",
  "video/mp4;codecs=avc3.64003E,opus",
  "video/mp4;codecs=hvc1.1.6.L186.B0,mp4a.40.2",
  "video/mp4;codecs=hvc1.1.6.L186.B0,opus",
  "video/mp4;codecs=hev1.1.6.L186.B0,mp4a.40.2",
  "video/mp4;codecs=hev1.1.6.L186.B0,opus",
  "video/mp4;codecs=av01.0.19M.08,mp4a.40.2",
  "video/mp4;codecs=av01.0.19M.08,opus",
];

for (const type of types) {
  console.log(
    `Is ${type} supported? ${
      MediaRecorder.isTypeSupported(type) ? "Yes!" : "Nope :("
    }`,
  );
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [MediaStream Recording API](/en-US/docs/Web/API/MediaStream_Recording_API)
- [Using the MediaStream Recording API](/en-US/docs/Web/API/MediaStream_Recording_API/Using_the_MediaStream_Recording_API)
- [Guide to media types and formats on the web](/en-US/docs/Web/Media/Guides/Formats)
- [Codecs in common media types](/en-US/docs/Web/Media/Guides/Formats/codecs_parameter)
- {{domxref("MediaStreamTrack")}}
- {{domxref("MediaStream")}}
- {{domxref("MediaCapabilities")}}
