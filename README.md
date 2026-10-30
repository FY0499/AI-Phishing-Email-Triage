# AI Phishing Email Triage

I built this n8n workflow to analyze incoming emails and identify potential phishing attempts using AI. It checks suspicious indicators, assigns a risk score, records the analysis, and sends an alert when needed.

<img width="729" height="189" alt="AI Phishing Email Triage workflow demo" src="https://github.com/user-attachments/assets/b03428e0-83ee-452e-9d72-7e019f39af36" />

## How it works

1. Gmail Trigger receives an incoming email.
2. The workflow extracts the sender, subject, message text, and links.
3. Gemini analyzes the email and returns a risk score and warning signs.
4. The result is checked and recorded in Google Sheets.
5. Potential phishing emails trigger a Telegram notification.

## Technologies

n8n, Gmail, Google Gemini, JavaScript, Google Sheets, and Telegram.

## Setup

Import [workflow.json](./workflow.json) into n8n, connect Gmail, Gemini, Google Sheets, and Telegram, and configure your phishing log sheet and alert destination.
