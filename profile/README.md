# Codeminity 🚀

An open-source ecosystem for building better software with less complexity.

## About

Codeminity creates reusable tools, libraries, and solutions that help developers build software faster, cleaner, and more efficiently.

We focus on improving developer experience through well-designed, maintainable, and practical open-source projects.

## Vision

Software development should be about solving problems and creating value — not repeating the same work over and over.

Codeminity aims to reduce complexity, encourage reuse, and help developers focus on what matters.

## Projects

All packages live in a single monorepo, [`ts-platform`](https://github.com/codeminity/ts-platform), organized by category. Each category below gets its own table as it grows — see that repo's `ARCHITECTURE.md` for how packages within a category relate to one another.

### 🌐 Request Layer

Framework-agnostic request infrastructure: authentication lifecycle, token refresh coordination, retry strategies, and safe async concurrency — shared by a family of adapters, one per HTTP client.

| Package | Description | Version |
| --- | --- | --- |
| [`@codeminity/request-core`](https://github.com/codeminity/ts-platform/tree/main/packages/request/core) | Framework-agnostic core primitives. Implements no HTTP transport itself — the shared foundation every adapter below builds on. | [![npm](https://img.shields.io/npm/v/@codeminity/request-core.svg)](https://www.npmjs.com/package/@codeminity/request-core) |
| [`@codeminity/axios`](https://github.com/codeminity/ts-platform/tree/main/packages/request/axios) | Production-ready Axios adapter. Same familiar Axios API, with a deterministic lifecycle layer on top. | [![npm](https://img.shields.io/npm/v/@codeminity/axios.svg)](https://www.npmjs.com/package/@codeminity/axios) |
| [`@codeminity/fetch`](https://github.com/codeminity/ts-platform/tree/main/packages/request/fetch) | Native `fetch` adapter. Same call signature and resolve/throw contract as `fetch` itself — no added surface to learn. | [![npm](https://img.shields.io/npm/v/@codeminity/fetch.svg)](https://www.npmjs.com/package/@codeminity/fetch) |

More categories and packages are coming soon.

## Examples

Real, runnable example applications demonstrating how to consume the published `ts-platform` packages as real npm dependencies — see [`ts-platform-examples`](https://github.com/codeminity/ts-platform-examples).

## Philosophy

Build less. Create more.

## Contributing

We welcome developers who share our passion for creating better tools and improving the software ecosystem.

If you are interested in contributing, feel free to explore our repositories, open issues, and submit pull requests.

---

© Codeminity
