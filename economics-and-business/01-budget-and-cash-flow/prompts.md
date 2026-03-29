# Module 01 — Prompt Card

## Before You Start

Open your terminal in this folder. Make sure `helix-labs-financials.csv` is in the same directory. Then start Claude Code:

```
claude
```

---

## Step 1: Load the Data and Understand the Business

Paste this into Claude Code:

```
Read the file helix-labs-financials.csv. This contains 3 months of financial data for Helix Labs, a UK SaaS startup selling project management software to construction firms.

Summarise what you see:
- Total monthly revenue for each month
- Total monthly costs for each month
- Monthly burn rate (costs minus revenue)
- Cash runway (how many months until the bank balance hits zero at current burn rate)

Present the summary as a clean table. Don't round — I need exact figures.
```

**What to look for in the output:**
- Is the company profitable in any month?
- Is the burn rate stable, increasing, or decreasing?
- How many months of cash runway remain?

**If something doesn't look right**, ask Claude: "Check your calculation for [month] — walk me through it line by line." This is what a real analyst does. You verify before you present.

---

## Step 2: Build the 12-Month Forecast

```
Using the 3 months of actuals from helix-labs-financials.csv, build a 12-month cash flow forecast from April 2026 to March 2027.

Assumptions for the BASE CASE:
- SME subscription revenue grows at the average monthly growth rate from the actuals
- Enterprise revenue stays flat at £8,500/month (existing contracts)
- Churn: lose 1 SME client per month (average from Q1 data)
- Fixed costs stay constant (salaries, rent, licences, insurance)
- Variable costs scale proportionally with revenue
- No new enterprise deals
- No additional fundraising

Output a month-by-month table showing:
- Total revenue
- Total costs
- Net cash flow (revenue minus costs)
- Closing cash balance

Highlight the month where cash hits zero (if it does).
```

**After reviewing the output, challenge it:**
- "What happens if churn increases to 4% per month instead of 2.5%?"
- "Are you accounting for the recruitment cost as a one-off or recurring?"
- "The commission calculation — is that on total revenue or new revenue only?"

---

## Step 3: Build the Optimistic and Pessimistic Scenarios

```
Now create two additional scenarios alongside the base case:

OPTIMISTIC SCENARIO:
- Everything in the base case, PLUS:
- Helix Labs wins both enterprise prospects in month 5 (adds £8,500/month from month 5 onwards)
- SME growth rate increases to 5% monthly (stronger product-market fit)
- Churn drops to 1.5% (enterprise clients reduce overall churn)

PESSIMISTIC SCENARIO:
- Everything in the base case, PLUS:
- Hargreaves Construction (biggest client, £4,250/month) churns in month 4
- SME growth rate slows to 1.5% monthly
- Marketing spend increases by £2,000/month from month 3 (trying to compensate)
- One developer leaves; replacement costs £3,000 in recruitment

Show all three scenarios side by side. For each scenario, tell me:
1. Which month does Helix run out of cash (if at all)?
2. What is the closing cash balance at month 12?
3. When does the company break even (monthly revenue exceeds monthly costs)?
```

---

## Step 4: Write the Executive Summary

```
Write a one-page executive summary for the Helix Labs board. The audience is non-financial — the board includes the founder, two angel investors (one is a construction industry veteran, one is a tech investor), and an independent advisor.

Structure:
1. HEADLINE — one sentence: what's the financial position?
2. KEY NUMBERS — the 3-4 figures the board must know
3. THREE SCENARIOS — one paragraph each, plain English, no jargon
4. BREAK-EVEN — when does it happen in each scenario and what drives it?
5. RECOMMENDATION — should Helix raise money, cut costs, or stay the course? Be specific and defend the recommendation.

Write in a professional but direct tone. No filler. Every sentence should contain a number or a decision.
```

**After reviewing, iterate:**
- "The recommendation needs to be stronger — what specific costs would you cut and how much would that save?"
- "The tech investor will ask about unit economics. Add a line about customer acquisition cost vs lifetime value."
- "Rewrite the headline — it's too soft. The board needs to know if this is urgent."

---

## Step 5: Reflect (2 minutes)

Don't skip this. Ask Claude:

```
I just completed a cash flow forecasting exercise. In a real FP&A analyst role, what would I do next with this analysis? What questions would my CFO ask that I haven't answered yet?
```

Write down the answer. This is the gap between "I built a forecast" and "I understand financial planning."

---

## What You Just Learned

| AI Skill | What You Practised |
|----------|-------------------|
| Structured briefing | Giving Claude specific parameters, assumptions, and output format |
| Data analysis | Loading and interpreting real financial data |
| Scenario modelling | Changing assumptions to see different futures |
| Output iteration | Challenging Claude's work and asking for revisions |
| Professional communication | Translating numbers into board-level plain English |
| Critical judgment | Questioning assumptions, verifying calculations |

---

## What a Recruiter Would Call This

If you're writing a CV, personal statement, or LinkedIn profile:

> "Built a three-scenario cash flow forecast for a SaaS startup using AI-assisted financial analysis. Produced an executive summary with break-even analysis and a funded recommendation for the board."

That's not a school exercise. That's a real skill.
