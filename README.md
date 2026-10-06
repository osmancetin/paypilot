# PayPilot

**An AI treasury controller for cross-border SMEs.** It decides what to fund, convert, defer or escalate when cash is short, and moves money only through coded rules after a human approves.

Built for the Airwallex Agentic Banking Hackathon, Kit 01: Adaptive Treasury Controller.

## The problem
Small businesses paying suppliers and staff in several currencies make weekly treasury decisions in spreadsheets, under time pressure. When cash is tight, mistakes are costly: late payroll, missed supplier terms, poor FX timing, duplicate payments.

## How PayPilot works
1. Reads multi-currency balances, upcoming obligations and FX quotes from Airwallex.
2. Recommends a decision for each obligation, with its reasoning.
3. A deterministic policy engine enforces hard rules: critical payments first, reserve floors, approval thresholds, no duplicates.
4. A human approves, and only then does code execute the conversion or payout.
5. Every recommendation, approval and API call is written to an audit log.

**Design principle:** the model proposes, the code decides, the API moves the money.

## Planned stack
TypeScript · Claude (tool use) · Airwallex sandbox APIs · SQLite · Next.js

## Status
📝 Idea stage. Build starts with the official hackathon period (Oct 25, 2026).
