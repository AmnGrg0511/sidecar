# Sidecar

Editor extension that brings an AI assistant into your code, grounded in the files you are working on. Type `@` to pull a file from the workspace into context, so answers come from your real code rather than guesswork.

## Highlights
- React webview experience inside VS Code
- `@file` context injection with workspace search, exclude patterns and a result cap
- Commands to open chat and set the Gemini API key
- Lightweight TypeScript + esbuild bundle

## Developer Notes
- Commands: `sidecar.open`, `sidecar.setGeminiApiKey`
- Webview UI lives in `webview-ui/`

## Tech Stack
- VS Code Extension API
- TypeScript
- React (webview)
- esbuild
