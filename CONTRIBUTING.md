# Contributing

Thank you for your interest in contributing!

## Getting started

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Commit using [Conventional Commits](https://www.conventionalcommits.org/)
5. Open a Pull Request

## Development setup

This project requires **Node.js v18** (it uses experimental React Server Components APIs).

```bash
git clone https://github.com/xabierlameiro/react-server-components.git
cd react-server-components
npm install
```

## Running the app

```bash
# Build the server and client bundles
npm run bundler:prod

# Start the server
node server.js
```

Open [http://localhost:4000](http://localhost:4000).

## Architecture

This is an experimental demo of React Server Components (pre-release):
- **Server** — Node.js + Express serves React Server Components
- **Client** — webpack bundles the client-side React
- **Data** — markdown notes stored on the filesystem

> **Note**: This uses pre-release React APIs (`react-fetch`, `react-pg`, `react-fs`) that are **not production-ready**.

## Reporting bugs

Open a [GitHub issue](https://github.com/xabierlameiro/react-server-components/issues).

## Questions

Reach out to [@xabierlameiro](https://github.com/xabierlameiro).
