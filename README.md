# TypeScript Chrome Extension

Chrome browser extension built with TypeScript. Demonstrates the full extension architecture — background service worker, content scripts, popup UI, and Chrome API integration — with strict typing throughout.

## Features

- Background service worker for persistent state and API calls
- Content script injection with DOM manipulation
- Popup UI built with TypeScript and vanilla CSS
- Chrome Storage API for persistent user preferences
- Context menu integration
- Message passing between extension components

## Tech Stack

| Component | Technology |
|---|---|
| Language | TypeScript 5 |
| Build | Webpack 5 |
| Chrome APIs | Manifest V3 |
| UI | Vanilla HTML/CSS |

## Getting Started

```bash
npm install
npm run build
```

Load into Chrome:
1. Open `chrome://extensions/`
2. Enable **Developer mode**
3. Click **Load unpacked** → select the `dist/` folder

## Development

```bash
npm run watch   # Rebuild on file changes
```

Reload the extension in `chrome://extensions/` after each build.

## Structure

```
src/
├── background/     # Service worker
├── content/        # Content scripts
├── popup/          # Extension popup UI
└── shared/         # Shared types and utilities
```
