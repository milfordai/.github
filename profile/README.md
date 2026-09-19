<p align="center">
  <img src="https://raw.githubusercontent.com/milfordai/.github/main/profile/logo.png" alt="Milford" width="96" />
</p>

<h1 align="center">Milford</h1>

<p align="center">
  <b>Intelligent workflows as code.</b><br />
  Typed decisions, model calls and HTTP calls in a graph you can read, version and test.
</p>

<p align="center">
  <img alt="License: Apache-2.0" src="https://img.shields.io/badge/license-Apache--2.0-007DCC" />
  <img alt="Status: early development" src="https://img.shields.io/badge/status-early%20development-FFB900?labelColor=1c1c1c" />
  <img alt="MCP: server and client" src="https://img.shields.io/badge/MCP-server%20%2B%20client-D10056" />
</p>

## What Milford is

Milford is a headless workflow engine. You describe a flow as plain JSON: small steps such as a typed decision, a model call, a template or an HTTP call, wired in a graph. Milford runs it behind an HTTP API, an MCP server, Slack, Telegram and webhooks, or as a TypeScript library.

It is not an agent framework. A flow is a fixed graph with no agent loop. Models answer narrow, typed questions, and your graph decides what happens next.

- **Typed decisions:** `choice`, `score` and `noul` answers with confidence, instead of parsed free text.
- **Any model:** OpenAI-compatible servers, Anthropic, Jev or your own classifier, with fallback, circuit breaker and rate limit.
- **MCP both ways:** expose flows as tools to LLM clients, and call other MCP servers from a flow.
- **One Docker image, no database:** for `linux/amd64` and `linux/arm64`.

## Get started

```bash
npx @milfordai/server milford.config.yaml
```

The packages are on npm under [`@milfordai`](https://www.npmjs.com/org/milfordai), and the documentation is at [milford.mintlify.site](https://milford.mintlify.site).

## Repositories

| Repository | What it is |
| --- | --- |
| [**milford**](https://github.com/milfordai/milford) | The engine, the HTTP and MCP servers, providers and channels. Apache-2.0. |

Runnable examples will follow in a separate repository.

## Status

Milford is in early development. The first release, 0.0.3, is on npm, and the config format can still change.

## Get in touch

Open an issue on the repository the question is about. To report a security problem, use the private vulnerability reporting on that repository instead of a public issue.
