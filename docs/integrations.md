# Integrations

[Home](../README.md) · [AI assistants](ai/README.md) · [Roadmap](../roadmap.md)

## Calendar providers

| Provider | Status | Connection and ownership |
| --- | --- | --- |
| [Google Calendar](https://www.comingup.today/integrations/google-calendar) | Available | Authorize a Google connection and choose calendars for read-only visibility |
| [iCloud Calendar](https://www.comingup.today/integrations/icloud-calendar) | Available | Connect with an Apple Account identifier and app-specific password for read-only visibility |
| Microsoft 365 / Outlook | Deferred | Not currently available |
| ICS, iCal, and additional provider ingestion | Exploring | No general import or provider-support commitment |

Connected calendars remain externally owned. ComingUp does not write changes
back to Google or iCloud events. ComingUp-created events have their own editing
workflow. Connections and visible-calendar selections are managed in the app;
provider update timing can vary.

Use the linked setup pages for current instructions and
[pricing](https://www.comingup.today/pricing) for connected-account and calendar
limits. Enter provider credentials only in the relevant connection flow, never
in a public issue or assistant conversation.

## AI assistants and MCP

ComingUp offers a hosted remote MCP endpoint for compatible assistants. It is
separate from calendar-provider authorization and requires its own approved
permissions. See [AI assistants](ai/README.md) and the [MCP reference](ai/mcp.md).

## Screens and photos

Household Display runs in a browser on existing hardware. Native Google Nest Hub
and Amazon Alexa/Echo Show integrations remain deferred.

Ambient Photos use selected uploads managed by ComingUp. A Google Drive folder
prototype was evaluated but is not the current photo integration. See the
[product decisions](https://www.comingup.today/roadmap/not-pursuing) for context.
