# Pricing Models and Paywalls

`marketing` · `pricing` · `glossary` · **Level:** Beginner

> [!NOTE]
> Plain-English definitions of the ways an app can charge money — paywall, freemium, free trial, and bundle — so the strategy docs make sense.

---

## What it is

A **pricing model** is simply the rule for _when and how_ a user has to pay. The same app can make wildly different money depending on which model it uses. The four you need to know:

_The core pricing terms, everyday explanation first:_

| Term | Think of it as... | Precise meaning |
| :--- | :--- | :--- |
| **Freemium** | A free mobile game that constantly nags you to buy coins | The app is **free to use forever**; you pay only to unlock extras or remove limits. Most users never pay. |
| **Hard paywall** | A newspaper that shows you the headline but blocks the article until you subscribe | The app is **unusable until you subscribe**. No free version — pay to get in at all. |
| **Free trial** | "First month free, cancel anytime" on a streaming service | A hard paywall with a **free taster period**. The user is charged automatically when the trial ends unless they cancel. |
| **Bundle** | A cable-TV package — many channels, one bill | **Several products sold together for one price**, cheaper than buying each separately. Your "5–7 apps, one subscription" is a bundle. |

---

## Why / when to use it

The choice between **freemium** and **hard paywall** is the single biggest money decision, because of one number: **conversion rate** (the share of downloaders who become paying users — see [metrics.md](metrics.md)).

_How the same downloads turn into payers under each model:_

| Model | Typical download-to-paid conversion | What that means for 10,000 downloads |
| :--- | :--- | :--- |
| **Freemium** | ~**2.1%** | ~210 paying users |
| **Hard paywall** | ~**10.7%** | ~**1,070** paying users |

So "hard paywall vs freemium conversion" — the row you asked about — just means: _of the people who download, what fraction pays, and a hard paywall converts about 5× more of them._ The trade-off is that a hard paywall usually gets **fewer downloads** (people are scared off by paying up front), but the ones who stay are worth far more.

> [!IMPORTANT]
> Free trials soften the hard-paywall downside: the user gets in free, gets hooked, then is auto-charged. The best apps convert **60%+** of trial users into payers. For running a 3-day anonymous local trial then a combined register-and-subscribe gate, see [registration-trial-and-data-lockin.md](../registration-trial-and-data-lockin.md).

---

## Example

The same app, same 10,000 downloads, under three models — to see why the model matters more than almost anything else:

```text
Freemium:        10,000 downloads -> ~2.1% pay  -> ~210 subscribers
Hard paywall:    10,000 downloads -> ~10.7% pay -> ~1,070 subscribers
Trial + paywall: 10,000 downloads -> trial start -> ~60% convert from trial
```

For your bundle plan, hard paywall (optionally with a trial) is the recommended model, because the whole point is that the apps are usable **only after subscribing**. For how to disclose that requirement so users are not surprised, see [hard-paywall-transparency.md](../hard-paywall-transparency.md).

---

## Key points / gotchas

- **Freemium ≠ free.** It means free _to start_; the business still depends on the small fraction who pay.
- **Hard paywall trades download volume for conversion.** Fewer people try it, but far more of them pay.
- **A free trial is still a hard paywall** — just with a delayed first charge. It is the usual way to make hard paywalls less scary.
- **A bundle is about perceived value**, not a discount — "many apps, one price" is the story that justifies subscribing.

---

## Common mistakes

- **Assuming freemium makes more money because it is "more popular."** The ~2.1% conversion usually loses to a hard paywall's ~10.7% unless download volume is enormous.
- **Confusing free trial with free forever.** A trial charges automatically; freemium never forces a charge.
- **Picking a model by gut.** It is the highest-leverage number in the whole plan — decide it from conversion data, not feel.

---

## References

- [RevenueCat — State of Subscription Apps 2026](https://www.revenuecat.com/state-of-subscription-apps/)
- [Recurly — Bundling strategies](https://recurly.com/blog/how-to-optimize-subscription-based-pricing-with-bundles/)

---

> [!TIP]
> **TL;DR** — Freemium = free forever with paid extras (~2.1% pay); hard paywall = pay to get in at all (~10.7% pay); free trial = a hard paywall with a free taster that auto-charges; bundle = many apps for one price.
