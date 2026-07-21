<p align="center">
  <img src="https://raw.githubusercontent.com/ViewDescriptorProtocol/.github/main/profile/assets/logo.png" alt="View Descriptor Protocol logo" width="140">
</p>

<h1 align="center">View Descriptor Protocol</h1>

<p align="center"><strong>Server-driven template binding for cross-platform UI rendering.</strong></p>

<p align="center">
  A JSON descriptor tells any client — Android, iOS, browser, desktop — which
  templates render which data, using slots and template URIs. The server decides
  how its data is presented; each client fetches the named templates and renders
  them natively. The data payload stays clean, templates stay independently
  cacheable, and no client hardcodes a view again.
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ViewDescriptorProtocol/.github/main/profile/assets/vdp-flow-dark.svg">
    <img alt="How VDP works: an API server responds with data plus a view descriptor; the client fetches the named templates from a template server and composes them into natively rendered UI on Android, iOS, web, and desktop" src="https://raw.githubusercontent.com/ViewDescriptorProtocol/.github/main/profile/assets/vdp-flow-light.svg" width="680">
  </picture>
</p>

## Where to start

| Repository | What it is |
|---|---|
| [**VDP**](https://github.com/ViewDescriptorProtocol/VDP) | The specification — view descriptor format, transports, discovery, conformance — plus JSON Schemas and validated examples |
| [**golang-vdp-demo**](https://github.com/ViewDescriptorProtocol/golang-vdp-demo) | A working end-to-end demo in Go: API, template server, and BFF client talking real HTTP, with a trace panel showing the protocol at work |
| [**HTMT**](https://github.com/ViewDescriptorProtocol/HTMT) | HyperText Markup Templating — JSONPath-based `ht-*` attributes for binding data to HTML, a natural template language for VDP on the web |
| [**Website**](https://vdprotocol.org) | The rendered specification, schemas, and changelog |

## Status

VDP is an **early working draft** (v0.1, alpha). The specification is
feature-complete for v0.1 and the Go demo implements it end to end; feedback
and implementations are welcome.

Previously known as Representational View State Transfer (RVST).
