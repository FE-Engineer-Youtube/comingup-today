# Connecting an AI assistant with MCP

[Home](../../README.md) · [AI assistants](README.md) · [Privacy and sharing](../privacy-and-sharing.md)

MCP is a shared way for AI assistants to connect to apps like ComingUp. Usually,
you only need to follow your assistant's setup instructions and approve access.

## Start with your assistant's guide

Use the instructions for [ChatGPT](https://www.comingup.today/integrations/ai/chatgpt),
[Claude](https://www.comingup.today/integrations/ai/claude),
[Grok](https://www.comingup.today/integrations/ai/grok), or
[another assistant](https://www.comingup.today/integrations/ai/other).
Connection options vary by assistant and account.

If the setup asks for a **server URL** or **connection address**, use:

```text
https://api.comingup.today/mcp
```

Sign in to ComingUp when prompted and review what the assistant wants to access.
There is no ComingUp server software to download or run yourself.

## Try a simple question

After connecting, ask: “Use ComingUp to show my schedule for this weekend.”
If that works, try another question or an action from the [AI guide](README.md).
You may need to allow additional permissions for the assistant to make changes.

## If you cannot connect

- Check that your assistant and plan support connecting to apps through MCP.
- Follow the current setup guide and check that you copied the address correctly.
- Make sure you signed in to the intended ComingUp account and approved access.
- If the assistant can read information but cannot change it, review its permissions.

If your connection works, you can ask the assistant to help submit a bug report
or feature request with your permission. If you cannot connect, email
[support@comingup.today](mailto:support@comingup.today) with the assistant's name
and a description of what went wrong. See [Help and feedback](../support.md).
Do not send passwords or private household information.

## For people building a connection

If you are developing an assistant or connection, the
[public server details](https://api.comingup.today/.well-known/mcp/server-card.json)
list the available tools and their technical requirements. Most customers can
use the setup guides above.
