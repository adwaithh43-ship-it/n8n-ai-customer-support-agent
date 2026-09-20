# AI Customer Support Agent — n8n

An AI-powered customer support workflow built with **n8n**, an LLM, conversational memory, customer/order data tools, and HTTP-based integrations.

> This repository contains a sanitized portfolio version of an n8n workflow. Credentials, secrets, instance-specific identifiers, and training-environment URLs have been removed or replaced.

## What it does

The workflow provides a chat-based support agent that can:

- Understand customer questions with an LLM
- Maintain conversation context with memory
- Retrieve customer information from a data source
- Retrieve order information through a tool/API
- Use tools instead of inventing customer or order details
- Return concise customer-facing answers

## Architecture

```text
Customer
   │
   ▼
Chat Trigger
   │
   ▼
AI Agent ───────────────► LLM
   │
   ├────────────────────► Conversation Memory
   │
   ├────────────────────► Customer Data Tool
   │
   └────────────────────► Order / HTTP Tool
   │
   ▼
Customer Response
```

## Tech stack

- n8n
- AI Agent
- LLM integration
- Conversation memory
- HTTP/API tools
- Structured customer/order data

## Import

1. Install or open an n8n instance.
2. Import `workflow/ai-customer-support-agent.json`.
3. Create/connect the required credentials in n8n.
4. Replace any placeholder endpoints or data sources with your own.
5. Test with sample/fake customer and order data before connecting production systems.

## Security

This public version intentionally does **not** contain:

- API keys
- Bearer tokens
- Passwords
- Personal customer data
- Private n8n instance identifiers
- Academy/training credentials

**Never commit secrets directly into an n8n JSON export.** Use n8n Credentials or another secret-management mechanism.

## Production improvements

For production use, I would add:

- Authentication and authorization
- CRM/database integration
- Human-agent escalation
- Structured logging
- Retry and timeout handling
- Rate-limit handling
- Input validation
- Monitoring and error alerts
- Customer identity verification
- Separate development/staging/production credentials

## Portfolio context

This project demonstrates practical experience with:

- AI agents
- API integration
- workflow automation
- data retrieval
- conversational memory
- tool calling
- business-process automation

It is intended as a technical portfolio project rather than a drop-in production customer-support system.

## License

MIT
