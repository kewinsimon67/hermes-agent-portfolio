# Meta Ads Reporting Harness

## Purpose

Convert read-only advertising data into a concise, auditable marketing report while keeping external side effects disabled.

## Inputs

- Ad account identifier supplied at runtime
- Campaign identifier supplied at runtime
- Reporting period
- Account currency

## Retrieval stages

1. Account details: verify currency and account state.
2. Campaign details: verify objective and delivery status.
3. Campaign insights: establish authoritative spend and totals.
4. Ad-set insights: compare delivery structure.
5. Ad insights: compare creative delivery and conversion signals.
6. Creative metadata: review live copy, CTA, form, and destination.

## Validation rules

- Never report a raw budget integer before checking the account currency.
- Do not treat missing metrics as zero.
- Do not judge performance from extremely small samples.
- Treat campaign-level spend as authoritative when lower-level totals disagree.
- Separate verified metrics from interpretation and recommendations.
- Never edit, publish, pause, delete, or budget-change campaigns during reporting.

## Output stages

- Executive summary
- Lifetime performance table
- Ad-level comparison
- Creative and offer analysis
- Lead-quality recommendations
- Measurement plan
- Limitations and decision rules

## Verification

The output PDF is checked for:

- Valid PDF structure
- Expected page count
- Presence of title and key sections
- Absence of secrets and raw account identifiers
