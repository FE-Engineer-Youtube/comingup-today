# AI assistants

[Home](../../README.md) · [MCP reference](mcp.md) · [Privacy and sharing](../privacy-and-sharing.md)

ComingUp's remote MCP service lets a compatible assistant work with the household
information and actions you authorize. The assistant connects through ComingUp
sign-in and consent; it does not need your ComingUp password in the conversation.

## What you can ask

- “Use ComingUp to show our schedule for this weekend.”
- “Find the note about school pickup.”
- “Add milk and apples to our shopping list.”
- “Create a ComingUp event for soccer practice Thursday at 5 pm.”
- “Save this recipe privately in ComingUp.”

Available actions depend on the connection's permissions and your access in
ComingUp. External calendar events remain read-only. Supported writes apply to
ComingUp-owned events, lists, notes, contacts, and private recipes.

The connection does not provide permanent deletion of top-level household
records, photo access, billing changes, or household administration. Removing a
list item is a supported exception for list contents. Review proposed changes
and the permissions you grant.

## Choose a client

| Client | Current direction | Setup |
| --- | --- | --- |
| ChatGPT | Submitted for directory review; submission does not establish approval | [ChatGPT guide](https://www.comingup.today/integrations/ai/chatgpt) |
| Claude | Connection guidance available; directory approval is not confirmed here | [Claude guide](https://www.comingup.today/integrations/ai/claude) |
| Grok | Integration and compatibility work underway | [Grok guide](https://www.comingup.today/integrations/ai/grok) |
| Other MCP clients | Requires compatible remote transport and OAuth support | [Other-client guide](https://www.comingup.today/integrations/ai/other) |

Client support can vary with provider, plan, account, and release. Follow the
linked guides for current setup details. These entries are not a promise that
every client or account has been tested successfully.

## Registry and directory status

Reviewed **September 3, 2026**:

| Directory | Status | Public evidence |
| --- | --- | --- |
| Official MCP Registry | Published, active version 1.0.0 | [Registry entry](https://registry.modelcontextprotocol.io/v0.1/servers/io.github.FE-Engineer-Youtube%2Fcomingup-today/versions/1.0.0) |
| Smithery | Public listing available | [ComingUp Today on Smithery](https://smithery.ai/servers/fe-engineer/comingup-today) |
| Glama | Submitted for review; approval not confirmed | No approved listing recorded here |

The Registry and Smithery entries were checked publicly. ChatGPT and Glama
submission status reflects the maintainer's report. Publication or submission
does not prove provider approval, a completed OAuth connection, or successful
tool execution. Registry entries describe the hosted service; they do not make
the application source code public.

## Public discovery is separate from household access

The website also provides [llms.txt](https://www.comingup.today/llms.txt),
[expanded public product information](https://www.comingup.today/llms-full.txt),
and browser site tools where supported. Those browser tools explain the product,
search public pages, describe the current public page, and return plan details.
They do not read or change private household information.

For the service address, tool catalog, and discovery metadata, see the
[MCP reference](mcp.md).
