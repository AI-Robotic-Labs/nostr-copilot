# Nostr Copilot 🤖🟣

*Nostr Copilot is a framework that integrates the Nostr protocol, artificial intelligence (AI), and the Bitcoin ecosystem, connecting these three systems into one cohesive platform.
How It Works*

- The user creates an nsec (Nostr private key) and selects an LLM (Large Language Model) such as OpenAI, Mistral, DeepSeek, etc.
- The user then adds an API key locally using a .env file or via a third-party server, such as AWS.
- Once configured, the user has a fully functional AI Agent for Nostr.

### Default Options

- NIP-05 verification
- Lightning Network address
- Liquid Network address

## Agent example

```json
{
  "nsec": "nsec1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "relay": "wss://relay.nostr.example.com",
  "ai_agent": {
    "model": "mistral-7b",
    "provider": "xAI",
    "description": "A lightweight AI model optimized for Nostr interactions."
  },
  "api_key": "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "options": {
    "nip05": "user@domain.com",
    "lightning_address": "user@ln.example.com",
    "liquid_address": "liquid1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
    "enabled_features": [
      "post_generation",
      "content_moderation",
      "bitcoin_tx_monitoring"
    ]
  },
  "metadata": {
    "version": "1.0.0",
    "created_at": "2025-03-06T12:00:00Z",
    "updated_at": "2025-03-06T12:00:00Z",
    "owner": "npub1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
  }
}
``
