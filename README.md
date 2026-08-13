# Hopium

![banner](Assets/logo.jpg)

The open AI model that lives up to the hype. Built to be the best-paired brain for Copium, Hopium gives you a smart, free, no-account AI model that actually delivers when it counts.

## Why Hopium

Why settle for overpriced, gated AI models when Hopium is open, free, and built to pair with Copium. Hopium is the model that powers your Copium coding agent — giving you top-tier reasoning, coding, and problem-solving without subscriptions, waitlists, or required accounts.

## Features

- **Open model** - Fully open weights, inspectable and auditable
- **Free by default** - No credit card, no subscription, no account required
- **Copium-native** - Optimized to pair perfectly with Copium coding agent
- **Coding-first** - Trained for real-world software engineering tasks
- **Streaming responses** - Real-time token streaming for fast feedback
- **Local or hosted** - Run it yourself or use a hosted endpoint

## Supported Providers

| Provider | Model | Notes |
|----------|-------|-------|
| Hopium Hosted | hopium/latest | Free tier available, no API key needed |
| BYOK | hopium-custom | Bring your own OpenAI-compatible endpoint |
| Ollama | hopium | Run locally, fully offline |
| Copium Native | hopium | Built-in support in Copium extension |

## Quick Start

1. Install Copium extension
2. Open Settings (Ctrl+,) and search for "Copium"
3. Set provider to `hopium` or add your Hopium API key
4. Start coding with Copium + Hopium

### Using with Copium

Open the Copium chat and start chatting — Hopium is the default brain when you select the Hopium provider:

```
@copium implement a REST API with Express and TypeScript
```

## Configuration

| Setting | Default | Description |
|---------|---------|-------------|
| copium.provider | hopium | Model provider |
| copium.hopium.apiKey | (empty) | Hopium API key |
| copium.hopium.model | hopium/latest | Model ID |
| copium.byok.endpoint | https://api.hopium.ai/v1 | BYOK endpoint |
| copium.byok.apiKey | (empty) | BYOK API key |
| copium.byok.model | hopium-custom | BYOK model name |
| copium.ollama.model | hopium | Ollama model name |
| copium.telemetry.enabled | false | Opt-in telemetry |

## Commands

All Copium commands work with Hopium:

- `Copium: Start Agent Task` - Start a Copium agent task powered by Hopium
- `Copium: Explain Selection` - Explain the current selection
- `Copium: Fix Diagnostic` - Fix the current diagnostic
- `Copium: Apply Edit` - Apply an edit to the current file

## Chat Commands

- `@copium <prompt>` - Chat with Copium + Hopium
- `@copium /swarm <prompt>` - Spawn swarm agents powered by Hopium

## Development

```bash
pnpm install
npm run compile
npm test
```

## License

MIT

## Disclaimer

This project was developed with assistance from Kilo Code for bug finding, code review, and implementation support. Kilo Code helped identify issues, suggest fixes, and implement features throughout the development process.
