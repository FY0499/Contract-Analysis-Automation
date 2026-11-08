# Contract Analysis Automation

An n8n workflow that extracts key information from uploaded contract PDFs and uses AI to identify important obligations, dates, amounts, review clauses, and an overall risk level.

## How it works

1. A reviewer uploads a contract PDF through an n8n form.
2. The workflow extracts text from the PDF.
3. An AI agent reviews the extracted text and structures the amounts, key dates, obligations, clauses needing review, and overall risk.
4. The workflow processes the result for storage and reviewer follow-up.

## Technologies

- n8n
- PDF text extraction
- Google Gemini
- JavaScript
- Google Sheets
- Gmail

## Setup

1. Import workflow.json into n8n.
2. Configure the AI, Google Sheets, and Gmail credentials.
3. Connect your own storage sheet and reviewer email, then test with a non-confidential sample contract.
4. Treat AI output as an initial review aid, not legal advice.

## Notes

This repository contains the exported n8n workflow. Configure your own credentials and integrations in n8n before running it.
