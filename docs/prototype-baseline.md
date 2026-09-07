# SC Mobile Protection Portfolio Intelligence — Prototype Baseline

## Purpose

Demonstrate how a needs-intelligence capability can identify a material customer need before surfacing an insurance proposition. This is an internal demonstrator using synthetic data only; it is not a recommendation, quote, underwriting decision, or live SC Mobile feature.

## Source trace

| Source | Decision carried into prototype |
| --- | --- |
| Whitepaper | Needs-first decisioning, explainability, correction, defer/decline, adviser handoff, synthetic data, and separation of need detection from product matching. |
| Proposal deck | Simon, Alex, and Sarah as core personas; Understand → Engage → Convert → Learn narrative; product shortlist after need qualification. |
| Existing SC Mobile screens | Additional Invest & Insure and insurance-journey context. |
| Supplied `sg-bank-withus-transactions.jpg` | Current SC Mobile Pay & Transfer reference: blue-to-teal header, green-edged service grid, outlined action pills, transaction tabs, and lower navigation treatment. This is the source of truth for Sarah’s banking-app entry styling. |
| Official SC Singapore product pages, checked 7 Sep 2026 | Product names and broad public descriptions only. Product content must be refreshed before any external sharing. See [insurance catalogue](https://www.sc.com/sg/insurance/), [protection solutions](https://www.sc.com/sg/insurance/protection/), and [PRUWealth Plus](https://www.sc.com/sg/insurance/pru-wealth/). |

## Personas and deterministic illustrative calculations

| Persona | Signal and need | Base calculation |
| --- | --- | --- |
| Simon, 55 | Approaching retirement; projected retirement-income shortfall | `(desired monthly retirement income − forecast monthly income) × 12 × retirement years` → S$2,000/month / S$480,000 over 20 years. |
| Alex, 35 | Mortgage, dependants, and income-protection exposure | `(monthly essential costs × support months + mortgage balance + recovery reserve) − existing cover` → S$270,000. |
| Sarah, 30 | New dependant and future education objective | `education goal − existing education funds − projected future savings` → S$34,000. |

All inputs are editable in the prototype. Updates recalculate only the synthetic illustrative gap; no result is an affordability, eligibility, premium, risk, or suitability outcome.

## Required flow

1. Simon begins from a generic iPhone push notification, Alex begins from a personalised email-client message, and Sarah begins from a rebuilt SC Mobile banking home with a distinct animated in-app Portfolio Intelligence notification.
2. Nudge states why it appeared and why it matters.
3. Customer reviews the data and assumptions, adjusts inputs, or corrects an input.
4. Customer can explore suitable solution types and a sourced product shortlist, defer, decline, or request adviser support.
5. Defer/decline visibly suppresses the present insight for the demo session; reset restores the default state.
6. The guided flow uses the client-facing stages “Your outlook”, “Your scenario”, and “Ways forward”. “Your scenario” presents modern input cards with direct manipulation and immediate illustrative impact.
7. An optional Portfolio Intelligence conversational assistant opens as a focused chat sheet. It begins as an adviser-led explanation of the identified illustrative gap; pre-defined questions append a simulated exchange and reveal a “See ways forward” action at the appropriate point.

## Product-content policy

- Use real product names and only high-level information sourced from official Standard Chartered Singapore pages.
- Keep fit explanations illustrative and non-binding.
- Present adviser review for complex protection, retirement, and family-planning decisions.
- No premium, product-term, coverage, return, or eligibility figures appear unless explicitly verified against a current official source and approved for the demonstrator.

## Acceptance criteria

- Each persona opens on an SC Mobile-style home route and completes the flow without a network call.
- Each gap changes immediately and transparently when an assumption is edited.
- Why-shown, data/assumptions, correction, defer, decline, shortlist, adviser handoff, and reset are all reachable by keyboard and pointer.
- The presentation remains a portrait handset on common laptop viewports.
