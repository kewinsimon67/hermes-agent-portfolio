# Hermes Agent Portfolio

A sanitized portfolio project demonstrating how I use an AI agent harness to turn read-only advertising data into decision-ready marketing analysis.

## What this showcases

- Tool-driven Meta Ads reporting
- Campaign, ad-set, and ad-level data retrieval
- Currency normalization and metric validation
- Creative and lead-quality analysis
- Separation of verified data, interpretation, and recommendations
- PDF report generation and verification
- Read-only safety boundaries: no campaign edits, publishing, or budget changes
- External-action safety: sensitive client/account data is excluded from this repository

## Workflow

1. Retrieve account currency and campaign status.
2. Retrieve campaign-level insights as the authoritative spend total.
3. Retrieve ad-set and ad-level delivery data.
4. Retrieve live creative metadata for copy review.
5. Normalize budgets and spend into the account currency.
6. Identify patterns, limitations, and lead-quality risks.
7. Generate a structured PDF report.
8. Verify the PDF file, page count, and key report text.

## Harness design

The harness is designed around controlled tool use rather than unsupported assumptions. Each stage has a defined input, output, validation rule, and safety boundary. Recommendations are generated only after the data and uncertainty are stated.

## Repository contents

- `reports/` — sanitized sample report and report notes
- `harness/` — workflow and safety documentation
- `docs/` — portfolio explanation of the method

All client names, account identifiers, campaign identifiers, creative copy, and sensitive performance details are anonymized or redacted.

## Important note

This is a portfolio demonstration. It does not contain access tokens, credentials, private Hermes configuration, memories, cron databases, or raw client account exports.
