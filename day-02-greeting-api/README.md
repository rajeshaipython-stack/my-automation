# Day 2 · Workflow 10 — Personal Greeting API (Webhook)

**What it does:** A live API that takes a name as a query parameter and returns a
personalized greeting plus a random fact. Visit `/webhook/hello?name=Rajesh` and
it replies "Hello Rajesh! …".

## Nodes
| Node | Type | Role |
|------|------|------|
| Webhook | Webhook (GET) | Live endpoint; reads the `?name=` query parameter |
| Get Fact | HTTP Request | Fetches a random fact |
| Build Reply | Edit Fields (Set) | Builds a personalized message (name + fact) |
| Respond | Respond to Webhook | Returns the greeting to the caller |

## Concepts learned
- **Webhook input** — reading query parameters from the incoming request
  (`$('Webhook').item.json.query.name`), i.e. accepting user input.
- **Referencing any node** — pulling data from any earlier node with
  `$('NodeName')`, not just the previous one.

## Run it
Import → **Publish** → open `/webhook/hello?name=YourName` → get a personalized reply.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
