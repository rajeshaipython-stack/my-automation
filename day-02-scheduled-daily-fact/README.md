# Day 2 — Scheduled Daily Fact

**What it does:** Every day at 9:00 AM, this workflow automatically fetches
a random fact from a public API and formats it into a clean message —
fully hands-free, running 24/7 on my self-hosted n8n server.

## Nodes
| Node | Type | Role |
|------|------|------|
| Every Day 9AM | Schedule Trigger | Fires automatically every day at 09:00 |
| Get Fact | HTTP Request | GET uselessfacts.jsph.pl random fact API |
| Format | Edit Fields (Set) | Builds message: "📚 Did you know? {text}" |

## Concept learned
**Schedule Trigger** — running automations automatically on a timer,
with no manual action needed.

## Run it
Import → **Execute workflow** to test → toggle **Active** to run daily.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
