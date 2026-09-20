# Security

Do not commit API keys, access tokens, passwords, webhook secrets, or private customer data.

For n8n, configure credentials through the n8n credential system rather than hard-coding them inside workflow nodes.

If a secret is accidentally committed, revoke/rotate it immediately and remove it from the repository history.
