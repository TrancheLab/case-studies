# TrancheLab Case Studies

Public capital structure extractions from Chapter 11 bankruptcy filings.

Every value is sourced to a specific page and sentence in the original filing.
Confidence scores are deterministic — never hallucinated.

## Cases

| Case | Debtor | Filed | Court | Tranches |
|------|--------|-------|-------|----------|
| 20-11218 | Hertz Corporation | May 22, 2020 | D. Del. | 6 |
| 22-11069 | Spirit Airlines | Nov 18, 2022 | D. Del. | TBD |

## Output Schema

Each extraction follows this schema:

```json
{
  "case_number": "20-11218",
  "debtor": "Hertz Corporation",
  "court": "U.S. Bankruptcy Court, D. Del.",
  "extracted_at": "2025-05-02T00:00:00Z",
  "extraction_time_seconds": 241,
  "tranches": [
    {
      "tranche": "First Lien Term Loan",
      "amount": "$656,000,000",
      "confidence": 0.75,
      "source_page": 312,
      "source_text": "..."
    }
  ]
}
```

## About TrancheLab

TrancheLab extracts capital structures from bankruptcy filings in minutes.
Built for restructuring professionals.

→ [tranchelab.com](https://tranchelab.com)
