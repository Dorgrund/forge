# Hard Paywall Transparency: Telling Users Before They Hit the Wall

`marketing` · `pricing` · `paywall` · `ux` · **Level:** Intermediate

> [!NOTE]
> What you can and cannot show users before download about a subscription requirement, why "free" apps with a hard paywall make users angry, and how to keep a hard paywall without the backlash.

---

## What it is

A **hard paywall** means the app is unusable until the user subscribes (see [pricing-models.md](terms/pricing-models.md)). The common complaint — users installing a "free" app and feeling tricked when they immediately hit a wall — is real, but it is a **disclosure and onboarding problem, not a reason to drop the hard paywall**. This doc covers the two separate decisions: how the **store** signals payment before download, and how **your app's first-open flow** sets honest expectations.

---

## Why / when to use it

Because the anger comes from **surprise**, not from paying. A hard paywall that is honest up front still converts at ~**10.7%** (vs ~2.1% freemium) and avoids the backlash. Apple now **actively rejects** apps with confusing or "dark pattern" paywalls, and both stores require price, terms, and renewal to be stated clearly. So transparency is both a trust win and a store-approval requirement.

---

## Example

Two separate decisions, kept distinct.

_Decision A — how the store shows payment before download:_

| Model | What the user sees in the store before installing | Trade-off |
| :--- | :--- | :--- |
| **Paid app** (upfront price) | Store shows a **price** instead of "Get/Install" — fully explicit | Honest, but kills downloads; a poor fit for subscriptions |
| **Free app + hard paywall** (the plan) | "Get/Install" (free). **Google Play** shows **"Offers in-app purchases"**; **Apple** shows a less prominent "In-App Purchases" section | Most downloads, but the paywall itself is not shown pre-install |

> [!IMPORTANT]
> You **cannot** make your full paywall screen appear in the store before download — neither store renders it pre-install. The strongest pre-install signals are Google's "Offers in-app purchases" label and Apple's IAP section, plus whatever you write in the **description and screenshots**. A true paid app is the only way to show a hard price upfront, and it is the wrong tool for a subscription.

_Decision B — the first-open flow, where the anger is actually solved:_

```text
Store listing  -> description + screenshots say plainly:
                  "Subscription required to use [App]"
First open     -> 2-3 onboarding screens showing the value
                  (time-to-value before the ask)
Paywall        -> states clearly: price, when charged,
                  renewal, how to cancel
                  (no toggles hiding the trial, no dark patterns)
```

This converts the high-intent users a hard paywall is meant to capture, and the explicit listing means nobody feels baited.

---

## Key points / gotchas

- **The store will not show your paywall before download.** The most explicit pre-install cue you control is the **description and screenshots** — state "subscription required" there.
- **Google Play labels in-app purchases more visibly** than Apple ("Offers in-app purchases" by the install button), but users rarely read either — your listing copy matters more.
- **A paid app is the only true upfront-price option**, and it is a bad fit for subscriptions (kills downloads, no recurring revenue).
- **The anger is a dark-pattern problem.** An honest hard paywall — clear price, clear renewal, value shown first — keeps the 10.7% conversion without the 1-star reviews.
- **Apple actively rejects confusing paywalls** (toggle-hidden trials, unclear terms) as of early 2026 — transparency is now also an approval gate.

---

## Common mistakes

- **Marketing the app as "free" with no hint a subscription is required** — the exact pattern that produces angry reviews and refund requests.
- **Assuming you can show the paywall in the store** — you cannot; only labels and your own copy appear pre-install.
- **Using a paid-app price to force transparency** — it solves surprise but destroys downloads and recurring revenue.
- **Hiding the trial or renewal behind toggles** — a dark pattern that triggers Apple rejection and user backlash.
- **Putting the paywall before any value** — show 2-3 screens of what the app does first, then ask.

---

## References

- [RevenueCat — Essential guide to mobile paywalls](https://www.revenuecat.com/blog/growth/guide-to-mobile-paywalls-subscription-apps/)
- [Adapty — How to design a paywall to pass App Store review](https://adapty.io/blog/how-to-design-paywall-to-pass-review-for-app-store/)
- [Airbridge — Hard vs soft paywalls](https://www.airbridge.io/en/blog/hard-vs-soft-paywalls)
- [Google Play Help — Make in-app purchases](https://support.google.com/googleplay/answer/1061913)

---

> [!TIP]
> **TL;DR** — You cannot show the paywall in the store before download (only a paid-app price or the "in-app purchases" label appears), so state "subscription required" in the listing description and screenshots, then use a short value-first onboarding and an honest paywall (clear price, renewal, cancel) — that keeps the hard paywall's ~10.7% conversion without the angry "I didn't know I had to pay" reviews.
