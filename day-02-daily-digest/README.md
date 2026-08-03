# Day 2 · Workflow 7 — Daily Digest (aggregate)

**What it does:** Fetches 5 posts and combines all their titles into a single
digest message — turning many items into one summary.

## Nodes
| Node | Type | Role |
|------|------|------|
| Start | Manual Trigger | Runs the workflow on click |
| Get 5 Posts | HTTP Request | Fetches a list of 5 posts |
| Combine Titles | Aggregate | Merges the `title` of all items into one list |
| Build Digest | Edit Fields (Set) | Joins the titles into a single digest message |

## Concept learned
**Aggregate** — combine many items into one. The opposite of item-by-item
processing. Real-world use: a daily digest, an orders report, or a summary of
all comments.

## Run it
Import → **Execute workflow** → the final node outputs one item: a digest of all 5 titles.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
