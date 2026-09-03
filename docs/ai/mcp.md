# MCP reference

[Home](../../README.md) · [AI assistants](README.md) · [Integrations](../integrations.md)

ComingUp runs a hosted Model Context Protocol (MCP) service. This repository
documents it; there is no local server package to install from this repository.

## Connection

| Setting | Value |
| --- | --- |
| Remote endpoint | `https://api.comingup.today/mcp` |
| Transport | Streamable HTTP |
| Authorization | OAuth through ComingUp sign-in and consent |
| Registry name | `io.github.FE-Engineer-Youtube/comingup-today` |
| Public setup guide | [AI integrations](https://www.comingup.today/integrations/ai) |

Add the remote endpoint using your client's supported connection flow, sign in
to ComingUp, and review the requested permissions. Start with a read such as
“What ComingUp account are you connected to?” before requesting changes.
Do not paste passwords or access/refresh tokens into chat.

## Discovery

- [Public server card and tool schemas](https://api.comingup.today/.well-known/mcp/server-card.json)
- [OAuth protected-resource metadata](https://api.comingup.today/.well-known/oauth-protected-resource/mcp)
- [OAuth authorization-server metadata](https://api.comingup.today/.well-known/oauth-authorization-server/oauth)
- [Official Registry record](https://registry.modelcontextprotocol.io/v0.1/servers/io.github.FE-Engineer-Youtube%2Fcomingup-today/versions/1.0.0)

The metadata can be read publicly. Tool calls through the remote endpoint require
OAuth, including tools that return public product information. Use the discovery
documents for protocol configuration rather than copying credentials or inventing
authorization URLs.

## Tool groups

The public server card exposed the following 28 tools on **September 3, 2026**.
Use its schemas and your connection's permissions as the current contract.

| Area | Read tools | Supported changes |
| --- | --- | --- |
| Published product information | `search_public_product_content`, `get_public_product_content` | None |
| Account and household context | `get_user_context`, `get_household` | None |
| Schedule and events | `get_schedule`, `find_events`, `get_event` | `create_event`, `update_event` |
| Lists | `get_lists`, `get_list` | `create_list`, `add_list_items`, `change_list`, `remove_list_item` |
| Notes | `find_notes`, `get_note` | `create_note`, `update_note` |
| Contacts | `find_contacts` | `create_contact`, `update_contact` |
| Recipes | `find_recipes`, `get_recipe` | `create_recipe`, `update_recipe` |
| Private support reports | `get_my_support_reports` | `submit_support_report` |

Tool discovery is not evidence that every action has been tested through every
assistant. Client-specific compatibility and directory review are tracked in the
[AI guide](README.md).

## Permissions and limits

The signed-in account and approved connection determine access. Tool arguments
cannot grant another household's permissions. Reads can return private content
to the connected AI provider; a note's sensitive-display setting is not an AI
access restriction.

Event changes apply only to ComingUp-owned events. Recipe writes remain private
and do not publish a recipe. Permanent deletion of top-level events, lists,
notes, recipes, contacts, or households is not exposed. List-item removal is
supported. Photos, billing changes, and household administration are outside
this connection's capabilities.

## Browser site tools

The website has a separate set of public, read-only WebMCP site tools:

- `get_comingup_today_overview`
- `get_current_comingup_page`
- `search_comingup_today`
- `get_comingup_today_pricing`

These help supported browsers discover public product information. They do not
provide private household access and are not another remote endpoint. Browser
support is optional; the site remains usable without it.
