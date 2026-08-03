# Day 2 · Workflow 6 — Smart Filter

**What it does:** Generates 10 random numbers and keeps only the ones greater
than 50, dropping the rest — demonstrating how to filter a list of data.

## Nodes
| Node | Type | Role |
|------|------|------|
| Start | Manual Trigger | Runs the workflow on click |
| Make 10 Numbers | Code | JavaScript loop creates 10 random numbers (1–100) |
| Keep only > 50 | Filter | Passes only items where value > 50, drops the rest |

## Concept learned
**Filter** — from a list of items, keep only the ones matching a condition and
discard the rest. (Unlike IF, which branches both paths, Filter keeps just one.)
Real-world use: keep only paid orders, high-priority leads, or emails from a
specific sender.

## Run it
Import → **Execute workflow** → only numbers > 50 pass through. Run again for a
different result.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
