<p align="center">
  <img src="https://raw.githubusercontent.com/ViewDescriptorProtocol/.github/main/profile/assets/logo.png" alt="View Descriptor Protocol logo" width="140">
</p>

<h1 align="center">View Descriptor Protocol</h1>

<p align="center"><strong>Server-driven template binding for cross-platform UI rendering.</strong></p>

<p align="center">
  A JSON descriptor tells any client — Android, iOS, browser, desktop — which
  templates render which data, using slots and template URIs. The server decides
  how its data is presented; each client resolves those template identifiers
  however its deployment chooses — a bundle inside the app, templates shipped
  with the page, a BFF-local store, or a remote fetch — and renders natively.
  The data payload stays clean, and no client hardcodes a view again.
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ViewDescriptorProtocol/.github/main/profile/assets/vdp-hub-dark.svg">
    <img alt="How VDP works: a view descriptor reaches any client — mobile, web, desktop, or a BFF — by any of several transports (HTTP Link header, inline _view/_views, View-Template header, well-known discovery); each template URL is an identifier the client resolves from any source — bundled in the app, shipped with the page, BFF-local, or fetched remotely — none of which is defined by VDP" src="https://raw.githubusercontent.com/ViewDescriptorProtocol/.github/main/profile/assets/vdp-hub-light.svg" width="720">
  </picture>
</p>

## Where to start

| Repository | What it is |
|---|---|
| [**VDP**](https://github.com/ViewDescriptorProtocol/VDP) | The specification — view descriptor format, transports, discovery, conformance — plus JSON Schemas and validated examples |
| [**golang-vdp-demo**](https://github.com/ViewDescriptorProtocol/golang-vdp-demo) | A working end-to-end demo in Go: API, template server, and BFF client talking real HTTP, with a trace panel showing the protocol at work |
| [**Website**](https://vdprotocol.org) | The rendered specification, schemas, and changelog |

## Status

VDP is an **early working draft** (v0.1, alpha). The specification is
feature-complete for v0.1 and the Go demo implements it end to end; feedback
and implementations are welcome.

Previously known as Representational View State Transfer (RVST).
