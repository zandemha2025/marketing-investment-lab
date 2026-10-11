# Marketing investment decision memo

Illustrative planning model — no measured customer results.

## Decision
Deploy $27000; keep $3000 unallocated (reserve plus channel ceilings). Forecast contribution: $67484 over 12 months. Expected customers: 9.8. CAC: 2743.

## Allocation
- Search: $12150; 4.8 expected customers; $33777 contribution
- Paid social: $8100; 1.5 expected customers; $5897 contribution
- Partner placements: $6750; 3.6 expected customers; $27810 contribution

## Sensitivity comparison
- Downside: CPC 20%; lead-rate -20%; contribution $35989
- Base: CPC 0%; lead-rate 0%; contribution $67484
- Upside: CPC -20%; lead-rate 20%; contribution $114726

## Experiment decision
Inconclusive: collect planned evidence. Absolute lift 5.0 percentage points; approximate 95% interval -2.6 to 13.0 pp. Practical threshold 2.0 pp.

## Assumptions and limits
Annual value $12000; gross margin 80%; all acquired customers start at horizon beginning. No cohort ramp, churn, attribution overlap, saturation, fixed costs, tax or sales costs. Channel CPC and rates are synthetic editable assumptions, not benchmarks. Fixed weights with ceilings leave budget unspent; no optimizer or causal forecast. Do not scale before checking sales capacity and incremental demand. Experiment assumes independent randomized users, a predeclared fixed window and one primary comparison; no repeated-peeking or multiple-testing correction.

## Experiment observations and gates
{
  "aN": 100,
  "aX": 5,
  "bN": 100,
  "bX": 10,
  "mde": 2,
  "complete": true,
  "guardrail": true
}

## Inputs (reproducible)
```json
{
  "budget": 30000,
  "reserve": 10,
  "acv": 12000,
  "margin": 80,
  "months": 12,
  "channels": [
    {
      "name": "Search",
      "weight": 45,
      "cpc": 8,
      "lead": 5,
      "qualified": 35,
      "win": 18,
      "cap": 16000
    },
    {
      "name": "Paid social",
      "weight": 30,
      "cpc": 5,
      "lead": 3,
      "qualified": 25,
      "win": 12,
      "cap": 12000
    },
    {
      "name": "Partner placements",
      "weight": 25,
      "cpc": 6,
      "lead": 4,
      "qualified": 40,
      "win": 20,
      "cap": 10000
    }
  ]
}
```
