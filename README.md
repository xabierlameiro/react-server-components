# React Server Components Demo

An experimental demo of React Server Components featuring a markdown notes app, built with Express, webpack, and pre-release React APIs.

[![CI](https://github.com/xabierlameiro/react-server-components/actions/workflows/ci.yml/badge.svg)](https://github.com/xabierlameiro/react-server-components/actions/workflows/ci.yml)

> **⚠️ Experimental**: This project uses pre-release React APIs (`react-fetch`, `react-pg`, `react-fs`) that are not production-ready. It is a learning resource for understanding React Server Components architecture.

## What it demonstrates

- React Server Components rendering on the server (no JS sent to the client)
- Client Components hydrated selectively
- Server-side data fetching with experimental `react-fetch`
- Webpack bundling for both server and client
- Per-component data colocation

## Stack

| Layer           | Choice                                       |
| --------------- | -------------------------------------------- |
| Runtime         | Node.js 18 + Express                         |
| UI              | React (experimental RSC build)               |
| Bundler         | webpack                                      |
| Data            | `react-pg`, `react-fs` (experimental)        |
| Fetch           | `react-fetch` (experimental)                 |
| Package name    | `react-notes` (internal)                     |

## Getting started

```bash
git clone https://github.com/xabierlameiro/react-server-components.git
cd react-server-components
npm install

# Build and start
npm run bundler:prod
node server.js
```

Open [http://localhost:4000](http://localhost:4000).

## Scripts

| Script                  | Description                           |
| ----------------------- | ------------------------------------- |
| `npm run bundler:prod`  | Build server + client bundles         |
| `npm run bundler`       | Build in watch mode                   |

## License

[MIT](./LICENSE) — © 2026 Xabier Lameiro
