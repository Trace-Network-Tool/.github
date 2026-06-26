<h1 align="center">Trace</h1>

<p align="center">
  <strong>A native proxy capture & API debugging toolkit for Apple platforms.</strong>
</p>

<p align="center">
  Inspect every request. Replay anything. Built end-to-end in Swift.
</p>

---

## 👋 Welcome

**Trace** is a network traffic inspector and API workbench for **iOS** and **macOS**. It combines a full HTTP/HTTPS/HTTP2 capturing proxy, TLS interception, WebSocket and SSE inspection, and a first-class request composer — all in native SwiftUI apps with no Flutter, CocoaPods, or web wrappers in the build graph.

Think of it as a debugging proxy and an API client living in the same app, sharing the same capture pipeline.

## ✨ What Trace Does

🔍 **Capture & Proxy**
- HTTP/1.1, HTTP/2, and HTTPS `CONNECT` capture built on SwiftNIO
- On-device TLS interception with a locally generated CA and per-host leaf certificates
- TUN-based packet capture for transport-level visibility on iOS
- WebSocket (incl. RFC 8441 over HTTP/2) and Server-Sent Events inspection
- gzip/deflate decoding, HAR & cURL import/export, search, favorites, history

🧪 **Compose — the API Workbench**
- Author, send, save, and organize requests into collections, folders, and environments
- Turn any captured request into an editable, replayable request
- Rich auth: API key, Basic, Bearer, JWT, OAuth 2.0 (PKCE/device/refresh), Digest, AWS SigV4, HMAC
- JavaScript pre-request / post-response scripting with a `pm.*` compatibility shim
- Flow & batch runners, assertions, timing waterfalls, diffs, and Markdown run reports
- Imports cURL, HAR, Postman, Insomnia, OpenAPI/Swagger; exports cURL, Postman, OpenAPI, Markdown

🛠 **Rules & Routing**
- Host mapping, rewrites, breakpoints, blocking, and scripted interceptors
- Direct, HTTP upstream, and SOCKS5 proxy routing
- Importable/exportable rule bundles

## 🧱 Built With

`Swift 6` · `SwiftUI` · `SwiftNIO` · `NIOSSL` · `NIOHTTP2` · `NetworkExtension` · `JavaScriptCore` · `Swift Certificates`

The codebase is organized as native app targets plus local Swift packages for capture, platform services, packet inspection, and a shared design system.

## 🚀 Status

Trace is in active development across iOS and macOS. Capture, TLS interception, the Compose workbench, WebSocket/SSE inspection, and rule engine are implemented and evolving.

---

<p align="center">
  <sub>Made with Swift for people who live in the network tab.</sub>
</p>
