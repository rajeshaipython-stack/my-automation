# Day 2 · Workflow 8 — Create a Post (HTTP POST)

**What it does:** Builds a small data object (title + body) and sends it to an
API using an HTTP POST request, which creates a new record and returns its id.

## Nodes
| Node | Type | Role |
|------|------|------|
| Start | Manual Trigger | Runs the workflow on click |
| Build Data | Edit Fields (Set) | Prepares the data to send (title + body) |
| Send (POST) | HTTP Request (POST) | Sends the data to the API to create a record |

## Concept learned
**HTTP POST** — sending/creating data, as opposed to GET which reads data.
This is how automations submit forms, create records, and push data to other
apps and databases.

## Run it
Import → **Execute workflow** → the POST node returns the created record with a
new `id`.

*Day 2 of my 30-Day n8n Automation Challenge 🚀*
