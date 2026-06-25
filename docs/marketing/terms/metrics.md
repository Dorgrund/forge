# Subscription Metrics

`marketing` · `metrics` · `glossary` · **Level:** Beginner

> [!NOTE]
> Plain-English definitions of the numbers that measure a subscription app — conversion, churn, ARPU, LTV, MRR — so the strategy docs make sense.

---

## What it is

These are the five numbers everyone in app subscriptions talks about. Each one answers a simple question about your money.

_The core metrics, everyday explanation first:_

| Term | The question it answers | Precise meaning |
| :--- | :--- | :--- |
| **Conversion rate** | "Of the people who download, how many pay?" | Share of downloaders who become paying subscribers. ~**2.1%** freemium, ~**10.7%** hard paywall. |
| **Churn** | "How many paying users quit each month?" | Share of subscribers who cancel in a period. Lower is better. |
| **ARPU** | "On average, how much does one user pay me?" | **A**verage **R**evenue **P**er **U**ser — total revenue ÷ number of users. |
| **LTV** | "How much is one customer worth over their whole life with me?" | **L**ife**t**ime **V**alue — total money a subscriber pays before they churn. ~**$23** global median after year 1. |
| **MRR** | "How much recurring money comes in each month?" | **M**onthly **R**ecurring **R**evenue — the predictable monthly subscription income. |

---

## Why / when to use it

These numbers connect to each other, and that chain is the whole business:

```text
downloads -> (conversion) -> subscribers -> (ARPU) -> monthly money (MRR)
subscribers stay longer  -> (low churn)  -> higher LTV -> more total money
```

So when a strategy doc says "hard paywall converts 5× better," it is talking about the **conversion** step. When it says "bundling reduces churn," it means subscribers **quit less often**, which raises **LTV**. Every lever in the plan is really pushing on one of these five numbers.

> [!IMPORTANT]
> **LTV must exceed what it costs to acquire a customer.** If a barter influencer's effort (free premium + revenue share) costs more than a subscriber's LTV, that channel loses money — these metrics are how you check.

---

## Example

A simple, made-up walk-through tying the metrics together:

```text
10,000 downloads
  x 10.7% conversion (hard paywall) = 1,070 subscribers
  x $6/month ARPU                   = ~$6,420 MRR
  average user stays ~6 months      = ~$36 LTV per subscriber
  5% monthly churn                  = ~50 subscribers lost each month
```

Reading it: conversion fills the top, ARPU sets the monthly value, churn drains the bottom, and LTV is the lifetime total. Reference points: median MRR one year after launch is only ~**$72**, and only ~**17.3%** of new apps ever reach **$1,000** MRR within two years.

---

## Key points / gotchas

- **Conversion and churn pull in opposite directions** — you want conversion high (more people pay) and churn low (they stay).
- **LTV is the "north star."** Almost every other metric exists to push LTV up; it is what tells you whether a marketing channel is profitable.
- **MRR is recurring, not one-off.** A $6 one-time sale is not MRR; a $6/month subscription is.
- **ARPU can be measured over all users or only payers** — check which one a source means before comparing.

---

## Common mistakes

- **Chasing downloads while ignoring conversion.** A million downloads at 0% conversion is $0.
- **Ignoring churn.** High churn quietly cancels out good conversion — you fill a leaky bucket.
- **Comparing LTV figures without the time window.** "LTV $23" usually means *after year 1*; lifetime-forever numbers differ.

---

## References

- [RevenueCat — State of Subscription Apps 2026](https://www.revenuecat.com/state-of-subscription-apps/)
- [RevenueCat — State of Subscription Apps 2025](https://www.revenuecat.com/state-of-subscription-apps-2025/)

---

> [!TIP]
> **TL;DR** — Conversion = % of downloaders who pay; churn = % who quit; ARPU = average pay per user; LTV = lifetime value of a customer; MRR = recurring monthly income — every strategy lever is really moving one of these five.
