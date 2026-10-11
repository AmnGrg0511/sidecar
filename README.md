# Sidecar

Editor extension that brings an AI assistant into your code, grounded in the files you are working on. Type `@` to pull a file from the workspace into context, so answers come from your real code rather than guesswork.

## Running it locally

```bash
git clone https://github.com/AmnGrg0511/sidecar.git
cd sidecar
npm run setup    # installs root and webview dependencies
npm run compile  # typecheck, lint and bundle
```

Then open the folder in VS Code and press `F5`, which launches an Extension Development Host with Sidecar loaded. Run `Sidecar: Open Chat`, then `Sidecar: Set Gemini API Key` to supply your key.

## Highlights
- React webview experience inside VS Code
- `@file` context injection with workspace search, exclude patterns and a result cap
- Commands to open chat and set the Gemini API key
- Lightweight TypeScript + esbuild bundle

## Developer Notes
- Commands: `sidecar.open`, `sidecar.setGeminiApiKey`
- Webview UI lives in `webview-ui/`
- `npm run setup` is required once before `npm run compile`; the webview is a separate npm project

## Tech Stack
- VS Code Extension API
- TypeScript
- React (webview)
- esbuild
