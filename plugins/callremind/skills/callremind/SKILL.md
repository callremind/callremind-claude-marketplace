---
description: Guide to using CallRemind from Claude Code — make automated AI voice calls, schedule reminders, and manage agents, leads, and notifications.
---

# CallRemind

CallRemind is automated AI voice call reminders (Malaysia, RM2 free credit on signup). Once
this plugin's MCP server (`https://mcp.callremind.my/mcp`) is connected, Claude Code can act
on your CallRemind account after you sign in.

## Quick start
- Ask Claude: *"Call my customer at +60123456789 and remind them about their appointment tomorrow."*
- Ask Claude: *"Schedule a reminder call for this Thursday 10am."*
- Ask Claude: *"Send a quick one-way reminder to +60123456789."* (uses Kokoro voice)

## What you can do
- **Instant call** — one-way voice call to any number (Edge/Kokoro TTS).
- **Quick call** — one-way notification, only a phone + message needed.
- **Schedule** — plan a reminder call for a future time.
- **Agents** — list/create/update AI agents and their voices.
- **Leads** — add/list contacts/leads.
- **Voice clones** — list/create clones.
- **Webhooks** — configure call events → your endpoint.
- **CEMAS** — emergency/notification callback destination + WhatsApp.
- **Reports & logs** — call analytics and history.

## Notes
- Sign in with your CallRemind account (email OTP, GitHub, or Google). A new account gets RM2 free credit.
- Messages are auto-checked for inappropriate language before they are spoken.
- Every action also maps to a REST API at `https://api.callremind.my/v1`.