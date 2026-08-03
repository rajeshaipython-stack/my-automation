# Day 2 · Workflow 4 — Number Checker (IF logic)

**What it does:** Generates a random number (1–100), checks whether it's greater
than 50, and routes to a "High" or "Low" branch accordingly — a simple
decision-making automation.

## Nodes
| Node | Type | Role |
|------|------|------|
| Start | Manual Trigger | Runs the workflow on click |
| Random Number | Code | JavaScript generates a random number 1–100 |
| Is it > 50? | IF | Splits the flow into two paths: True (>50) / False (≤50) |
| High | Edit Fields (Set) | Message when the number is HIGH (>50) |
| Low | Edit Fields (Set) | Message when the number is LOW (≤50) |

## Concepts learned
- **IF — conditional branching:** send the flow down different paths based on a condition (the core of decision-making automations).
- **Code node:** write custom JavaScript inside n8n (`Math.random()` to generate the number).

## Run it
Import → **Execute workflow** → only the matching branch (High *or* Low) lights up
green. Run it a few times to see it switch between paths.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
