# Day 2 · Workflow 3 — Live Fact API (Webhook)

**What it does:** A live public API endpoint. Anyone who visits the URL gets a
random fact back in real time, served 24/7 from my self-hosted n8n server.

## Nodes
| Node | Type | Role |
|------|------|------|
| Webhook | Webhook (GET) | Public trigger — fires when someone visits the URL |
| Get Fact | HTTP Request | Fetches a random fact from a public API |
| Respond | Respond to Webhook | Returns the fact to the caller as the response |

## Concept learned
**Webhook + Respond** — receiving requests from the outside world, running logic,
and returning a response. The foundation of APIs, chatbots, and integrations.

## Run it
Import → **Publish** (activate) → open the Production webhook URL → a fact is returned.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
