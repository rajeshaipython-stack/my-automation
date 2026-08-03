# Day 2 · Workflow 9 — Daily Bitcoin Price to Telegram

**What it does:** Every day at 9 AM, fetches the live Bitcoin price (USD + INR)
and sends it to my Telegram automatically. A real, useful automation combining
several concepts.

## Nodes
| Node | Type | Role |
|------|------|------|
| Every Day 9AM | Schedule Trigger | Fires daily at 09:00 |
| Get BTC Price | HTTP Request | Fetches live BTC price from CoinGecko |
| Build Message | Edit Fields (Set) | Formats the price message (reads nested JSON) |
| Send to Telegram | Telegram | Delivers the price to my Telegram |

## Concepts learned
- **Nested data access** — reaching into JSON-inside-JSON with dot notation
  (`$json.bitcoin.usd`).
- **Combining skills** — schedule + API + data formatting + delivery into one
  real, working automation.

## Run it
Import → connect the existing Telegram credential → set Chat ID → **Execute** to
test → **Activate** for a daily 9 AM price alert.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
