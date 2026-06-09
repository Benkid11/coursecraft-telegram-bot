# CourseCraft Telegram Bot

An n8n workflow that creates an AI-powered Telegram chatbot for the Eduvi/CourseCraft platform.

## Features

- Retrieval Augmented Generation (RAG) using Vector Store
- Integrates with Google Docs for course information
- Mistral Cloud embeddings for semantic search
- Support escalation with email capture
- Memory management for conversation context

## Setup Instructions

### Prerequisites

- n8n instance (Docker or self-hosted)
- Telegram Bot Token (from @BotFather)
- Google Docs API credentials
- Mistral Cloud API key

### Installation

1. Download the workflow JSON
2. In n8n, go to **Workflows** → **Import**
3. Upload the JSON file
4. Configure credentials:
   - Telegram API (with your bot token)
   - Google Docs (OAuth2)
   - Mistral Cloud API key

### Docker Setup

```bash
cd C:\n8n
docker compose up -d
.\ngrok.exe http 5678 --url https://your-ngrok-url.ngrok-free.dev
```

### Webhook Configuration

Update your `.env` file with:
