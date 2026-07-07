# 🚀 AI Radar

An automated n8n workflow that discovers trending AI tools from GitHub, researches them deeply using an AI Agent, and delivers a beautifully formatted report via email — every 6 hours, fully hands-off.

## How it works

1. **Discovery**: Scans GitHub Trending every 6 hours for new AI-related repositories
2. **Research**: An AI Agent analyzes each tool — what it is, why it was built, pricing, pros/cons, learning curve, alternatives, and monetization ideas
3. **Deduplication**: Cross-checks against previously sent tools using Google Sheets
4. **Delivery**: Sends a clean, formatted HTML email report
5. **Logging**: Tracks all sent tools in Google Sheets for history

## Tech Stack

- **n8n** — workflow orchestration
- **AI Agent (LLM)** — tool research & JSON-structured analysis
- **Google Sheets** — deduplication + logging
- **Gmail** — email delivery

## Workflow

![Workflow Screenshot](workflow-screenshot.png)

## Setup

1. Import the workflow JSON into your n8n instance
2. Connect your own credentials (Gmail, Google Sheets, AI model API key)
3. Update the Google Sheet ID in the "Get row(s)" and "Append" nodes
4. Activate the workflow

## Sample Output

*![Email Output](AI%20Radar%20Email%20output.jpeg)*

## Future Improvements

- [ ] Add Telegram notifications
- [ ] Add Notion integration
- [ ] Build a web dashboard for trending scores

---

Built as a personal automation project to stay updated with the fast-moving AI tools landscape.
