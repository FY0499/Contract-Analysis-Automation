# Contract Analysis Automation

I built this n8n workflow to extract important information from PDF contracts and use AI to organize key details that may need the reviewer's attention.

<img width="767" height="228" alt="Contract Analysis Automation workflow demo" src="https://github.com/user-attachments/assets/826e4601-4909-4d95-8882-528745583a2b" />

## How it works

1. The user uploads a contract PDF through a form and provides the legal reviewer's email address.
2. The workflow extracts the text from the uploaded document.
3. Google Gemini analyzes the contract and identifies financial amounts, important dates, obligations for each party, and clauses that need careful review.
4. JavaScript processes the AI response and prepares the review results.
5. The extracted information is saved to Google Sheets and sent to the reviewer by email.

## Main features

- PDF contract text extraction.
- AI analysis of amounts, dates, and obligations.
- Identification of clauses that may need further review.
- Overall contract risk classification.
- Google Sheets logging and email reporting.

## Technologies

n8n, Google Gemini, PDF extraction, AI Agent, JavaScript, Google Sheets, Gmail, and n8n Forms.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Gemini, Google Sheets, and Gmail credentials, then connect your review sheet and set the legal reviewer's email address. Test it with a non-confidential sample contract first.
