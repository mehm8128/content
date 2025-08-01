---
title: Pragma header
short-title: Pragma
slug: Web/HTTP/Reference/Headers/Pragma
page-type: http-header
status:
  - deprecated
browser-compat: http.headers.Pragma
sidebar: http
---

{{Deprecated_Header}}

The HTTP **`Pragma`** header is an implementation-specific header that may have various effects along the request-response chain.
This header serves for backwards compatibility with HTTP/1.0 caches that do not support the {{HTTPHeader("Cache-Control")}} HTTP/1.1 header.

> [!NOTE]
> The `Pragma` header is not specified for HTTP responses and is therefore not a reliable replacement for the HTTP/1.1 `Cache-Control` header, although its behavior is the same as `Cache-Control: no-cache` if the `Cache-Control` header field is omitted in a request.
> Use `Pragma` only for backwards compatibility with HTTP/1.0 clients.

<table class="properties">
  <tbody>
    <tr>
      <th scope="row">Header type</th>
      <td>
        {{Glossary("Request header")}},
        {{Glossary("Response header")}} (response behavior is not specified and is implementation-specific).
      </td>
    </tr>
    <tr>
      <th scope="row">{{Glossary("Forbidden request header")}}</th>
      <td>No</td>
    </tr>
    <tr>
      <th scope="row">
        {{Glossary("CORS-safelisted response header")}}
      </th>
      <td>Yes</td>
    </tr>
  </tbody>
</table>

## Syntax

```http
Pragma: no-cache
```

## Directives

- `no-cache`
  - : Same as `Cache-Control: no-cache`. Forces caches to submit the request to the origin server for validation before a cached copy is released.

## Examples

```http
Pragma: no-cache
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{HTTPHeader("Cache-Control")}}
- {{HTTPHeader("Expires")}}
