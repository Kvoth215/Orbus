# Real World Budget Challenge
### A High School Financial Literacy Simulation

A self-paced, browser-based simulation in which students are randomly assigned a real entry-level job, receive an accurate pay stub with taxes withheld, and navigate eight monthly spending stations to build — or bust — a budget.

---

## Live Demo

> Once deployed to GitHub Pages, replace this line with your link:
> **https://your-username.github.io/real-world-budget-challenge**

---

## Overview

| Detail | Info |
|---|---|
| **Subject** | Personal Finance / Business & Economics |
| **Grade Level** | High School (9–12) |
| **Format** | Self-paced, online, multi-day |
| **Time Required** | 2–3 class periods or assigned as independent work |
| **Tech Required** | Any modern browser — no login, no install |

---

## What Students Experience

### Phase 1 — Career Spin
Students spin a randomized job wheel and receive one of 12 real entry-level positions. Salaries are sourced from **U.S. Bureau of Labor Statistics (BLS) 2024** occupational data.

| Job Title | Annual Salary |
|---|---|
| Childcare Worker | $28,500 |
| Food Prep Worker | $29,000 |
| Home Health Aide | $30,000 |
| Retail Sales Associate | $33,000 |
| Security Guard | $34,500 |
| Warehouse Associate | $36,500 |
| Bank Teller | $37,500 |
| Customer Service Rep | $38,000 |
| Delivery Driver | $39,000 |
| Medical Assistant | $40,000 |
| Construction Laborer | $40,500 |
| Administrative Assistant | $42,000 |

### Phase 2 — Pay Stub
Students see their **gross monthly pay** broken down with four real deductions:
- **Federal income tax** — 2024 IRS brackets, standard deduction applied
- **Pennsylvania state income tax** — 3.07% flat rate
- **Social Security (FICA)** — 6.2%
- **Medicare** — 1.45%

The simulation surfaces the key insight that **12–20% of every paycheck** is withheld before the student ever sees a dollar.

### Phase 3 — Eight Spending Stations
A live budget tracker (net pay / spent / remaining) updates at every station.

| Station | Concept Covered |
|---|---|
| Housing & Rent | 30% housing rule, roommates vs. solo living |
| Transportation | True cost of a car vs. transit |
| Groceries & Food | Meal prep vs. eating out |
| Healthcare & Insurance | Consequences of being uninsured |
| Entertainment & Subscriptions | Subscription creep |
| Savings & Emergency Fund | 50/30/20 rule, percent-based savings |
| Student Loans & Debt | Education cost vs. earning potential |
| Clothing & Personal Care | Discretionary spending habits |

### Phase 4 — Budget Report & Reflection
Students receive a surplus or deficit result alongside a full income and expense breakdown. Six higher-order reflection questions prompt critical thinking beyond the simulation itself.

---

## How to Deploy (GitHub Pages — Free)

1. **Fork or clone** this repository to your GitHub account.
2. Go to **Settings → Pages**.
3. Under *Source*, select **Deploy from a branch**.
4. Choose **main** branch and **/ (root)** folder. Click Save.
5. GitHub will provide a URL (usually within 1–2 minutes).
6. Share that URL with students — no login required.

That's it. The simulation runs entirely in the browser with no server, no database, and no student accounts needed.

---

## Classroom Use

### Recommended Schedule

**Day 1**
- Introduce the simulation and its purpose
- Students complete Phase 1 (job spin) and Phase 2 (pay stub)
- Class discussion: What surprised you about your take-home pay?

**Day 2**
- Students complete all eight spending stations (Phase 3)
- Encourage students to genuinely consider each option rather than clicking through quickly

**Day 3**
- Students review their Phase 4 report and answer reflection questions in writing
- Class debrief (see teacher guide for discussion prompts)
- Optional: Have students re-run the simulation with a different job and compare outcomes

### Discussion Anchors
- Compare a student who received the Childcare Worker salary vs. the Administrative Assistant salary — how different were their choices?
- Who chose no health insurance? What did that save them monthly? Was it worth the risk?
- Which students saved 10% of their net pay? What did they give up to do it?

---

## Files

```
/
├── index.html          ← The complete simulation (single file, no dependencies)
├── README.md           ← This file
└── teacher-guide.md    ← Answer key, debrief guide, and extension activities
```

---

## Technical Notes

- **No external dependencies** — pure HTML, CSS, and vanilla JavaScript
- **No data is collected** — nothing is stored, transmitted, or tracked
- **Works offline** — can be saved and opened as a local file if needed
- **Mobile-compatible** — responsive layout works on tablets and phones
- **Tax calculations** update in real time based on each student's assigned salary using actual 2024 IRS federal tax brackets and Pennsylvania's 3.07% flat state income tax rate

---

## Customization

To adapt this simulation for another state, open `index.html` and find the `calcTaxes()` function. Update the `pa` line with your state's tax rate:

```javascript
// Example: change PA (3.07%) to NJ (varies) or NY (4%)
const pa = sal * 0.04 / 12;  // Replace 0.04 with your state's rate
```

To add or remove jobs, edit the `JOBS` array near the top of the script section.

---

## Standards Alignment

This simulation addresses the following common high school personal finance standards:

- Calculating gross vs. net income and understanding payroll deductions
- Creating and evaluating a personal budget
- Analyzing the relationship between education, career, and income
- Evaluating trade-offs in financial decision-making
- Understanding insurance and risk management

---

## Credits

- Salary data: [U.S. Bureau of Labor Statistics Occupational Employment Statistics, 2024](https://www.bls.gov/oes/)
- Tax data: [IRS Revenue Procedure 2023-34 (2024 tax year brackets)](https://www.irs.gov/) and Pennsylvania Department of Revenue
- Built for classroom use by a PA middle/high school Business & Computer Information Technology teacher

---

*Last updated: 2025 · Free for classroom use*
