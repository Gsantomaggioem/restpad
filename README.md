# restpad

Tiny REST API for saving and tagging bookmarks

Small but I use it weekly.

## Features

- env-driven port, runs anywhere Node does
- Request validation helpers, no framework magic
- In-memory store with optional JSON persistence
- REST endpoints: list / create / delete / search
- Morgan logging and centralized error handler

## Install

```bash
npm install
npm run dev
```

## Usage

```bash
curl -X POST localhost:3000/api/bookmarks \
  -H 'content-type: application/json' \
  -d '{"url": "https://example.com", "tags": ["reading"]}'
```

## Project structure

```text
├── docs/
│   ├── configuration.md
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   ├── config.js
│   ├── index.js
│   └── store.js
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
└── package.json
```

## Development

```bash
npm install
```

## Why

Needed this for myself; figured others might too.
