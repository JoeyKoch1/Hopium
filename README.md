# Hopium

![banner](Assets/logo.jpg)

The open AI model that lives up to the hype. Hopium gives you a smart, free, no-account AI model that actually delivers when it counts, built for developers who want real power without the price tag.

## Why Hopium

Why settle for overpriced, gated AI models when Hopium is open, free, and built for real work. Hopium is an open AI model giving you top-tier reasoning, coding, and problem-solving without subscriptions, waitlists, or required accounts.

## Features

- **Open model** - Fully open weights, inspectable and auditable
- **Free by default** - No credit card, no subscription, no account required
- **Coding-first** - Trained for real-world software engineering tasks
- **Streaming responses** - Real-time token streaming for fast feedback
- **Local or hosted** - Run it yourself or use a hosted endpoint
- **Easy integration** - OpenAI-compatible API, drop into any tool that speaks OpenAI

## Supported Providers

| Provider | Model | Notes |
|----------|-------|-------|
| Hopium Hosted | hopium/latest | Free tier available, no API key needed |
| BYOK | hopium-custom | Bring your own OpenAI-compatible endpoint |
| Ollama | hopium | Run locally, fully offline |

## Quick Start

1. Sign up at [hopium.dev](https://hopium.dev) or run locally with Ollama
2. Grab your API key from the dashboard
3. Point your tool of choice at `https://api.hopium.dev/v1` with model `hopium/latest`

### Using with any client

Hopium is OpenAI-compatible, so it works with any client that supports the OpenAI API:

```bash
curl https://api.hopium.dev/v1/chat/completions \
  -H "Authorization: Bearer $HOPIUM_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"model":"hopium/latest","messages":[{"role":"user","content":"Write a hello world in Python"}]}'
```

## Configuration

| Setting | Value | Description |
|---------|-------|-------------|
| API Endpoint | `https://api.hopium.dev/v1` | Hopium hosted endpoint |
| Model | `hopium/latest` | Latest Hopium model |
| API Key | (from dashboard) | Your free Hopium API key |
| Ollama Model | `hopium` | Local model name for Ollama |

## Integration Examples

### Python

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.hopium.dev/v1",
    api_key="your-hopium-api-key"
)

response = client.chat.completions.create(
    model="hopium/latest",
    messages=[{"role": "user", "content": "Write a hello world in Python"}]
)
```

### Node.js

```javascript
import OpenAI from 'openai';

const client = new OpenAI({
    baseURL: 'https://api.hopium.dev/v1',
    apiKey: 'your-hopium-api-key'
});

const response = await client.chat.completions.create({
    model: 'hopium/latest',
    messages: [{ role: 'user', content: 'Write a hello world in Python' }]
});
```

## Local Development

```bash
pnpm install
npm run compile
npm test
```

## License

MIT

## Pairing

Works best combined with Copium :D
