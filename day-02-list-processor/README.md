# Day 2 · Workflow 5 — List Processor (multiple items)

**What it does:** Fetches a list of 5 posts from an API and automatically formats
each one into a summary — demonstrating how n8n processes lists of data.

## Nodes
| Node | Type | Role |
|------|------|------|
| Start | Manual Trigger | Runs the workflow on click |
| Get 5 Posts | HTTP Request | Fetches a list of 5 posts from a public API |
| Format Each | Edit Fields (Set) | Builds a summary — runs once per item, automatically |

## Concept learned
**Multiple items** — when a node outputs a list, n8n runs the next node once for
*every* item automatically (no manual loop needed). This is fundamental, because
real-world data almost always arrives as lists.

## Run it
Import → **Execute workflow** → the Format node outputs 5 items, one summary each.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
