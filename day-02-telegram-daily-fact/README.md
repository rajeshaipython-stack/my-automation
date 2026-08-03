# Day 2 · Workflow 2 — Daily Fact to Telegram

**What it does:** Every day at 9:00 AM, this workflow automatically fetches a
random fact and delivers it straight to my Telegram — hands-free, running 24/7
on my self-hosted n8n server.

## Nodes
| Node | Type | Role |
|------|------|------|
| Every Day 9AM | Schedule Trigger | Fires automatically every day at 09:00 |
| Get Fact | HTTP Request | GET a random fact from a public API |
| Send to Telegram | Telegram | Sends the fact to my Telegram chat |

## Concept learned
**Credentials + Delivery** — connecting an external service (Telegram Bot API)
with a secure credential and delivering automation output to a real destination.

## Debugging note 🐞
Hit a `Bad Request: can't parse entities` error — the API text had a backtick (`)
which broke Telegram's Markdown parsing.
**Fix:** set the Telegram node **Parse Mode → HTML** (backticks aren't special in HTML).

## Setup
- Telegram bot via @BotFather (token stored as an n8n credential)
- Chat ID from @userinfobot

## Run it
Import → add Telegram credential → set Chat ID → Parse Mode = HTML →
**Execute** to test → **Activate** for daily delivery.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
