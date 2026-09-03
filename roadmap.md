# Roadmap

[Home](README.md) · [Features](docs/features.md) · [AI assistants](docs/ai/README.md)

This is a compact product-direction snapshot reviewed on **September 3, 2026**.
The [website roadmap](https://www.comingup.today/roadmap) carries the fuller
descriptions. Priorities may change; exploring and deferred items are not
delivery commitments.

## Shipped

- Public demo household with synthetic data.
- Today, Week, and Month views; ComingUp events and contacts.
- Read-only Google and iCloud calendars.
- Shared lists, item checkoffs, notes, and sensitive note presentation controls.
- Household recipes, deliberate public recipe/cookbook sharing, and print views.
- Recipe imagery performance and reliability improvements.
- Household Display, Ambient mode, and managed private photos.
- Optional weather context for supported U.S. locations.
- Installable PWA and opt-in web push reminders in supported browsers.
- Schedule revalidation on return to the foreground and supported in-app changes.
- Authenticated MCP access with permission-controlled reads and ComingUp writes.

## In focus

- **Photo Bomb:** explore an occasional multi-photo moment within Ambient mode
  that returns to the schedule-focused rotation.
- **AI compatibility and distribution:** continue provider testing and review.
  ChatGPT has been submitted, Grok work is underway, and MCP registry listings
  and submissions are progressing. See [dated status](docs/ai/README.md#registry-and-directory-status).

## Exploring

- Deliberate, opt-in sharing between separate households and extended families.
- More shared-display presentation controls for lists, events, and photos;
  potentially making Notes opt-in on newly configured displays.
- ICS/iCal and additional calendar ingestion.
- Responsibilities and day-anchored Today items with calm completion state.
- Richer context for managed photos.
- Household financial awareness, without bank-account aggregation as the core.
- Revocable read-only schedule links and small Today widgets.

## Deferred

- Microsoft 365 and Outlook calendars.
- Google Home/Nest Hub and Amazon Alexa/Echo Show integrations.
- Additional photo-provider imports and native apps without a clear product need.

## Product boundaries

ComingUp does not write back to external calendars. It is not pursuing household
behavior scoring, family gamification, a built-in chat platform, or medical-record
and compliance workflows. A Google Drive photo-folder prototype is not the
current photo approach.

SMS, geofencing, meal planning, and ingredient-to-list actions are not current
capabilities or delivery commitments. For the reasoning behind deliberate
decisions, see [Not pursuing](https://www.comingup.today/roadmap/not-pursuing).
