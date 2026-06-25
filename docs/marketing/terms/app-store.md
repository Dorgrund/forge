# App Store and Play Market Terms

`marketing` · `app-store` · `glossary` · **Level:** Beginner

> [!NOTE]
> Plain-English definitions of the App Store (Apple) and Play Market (Google) terms — commission, Small Business Program, SKU, offer codes — so the monetization strategy makes sense.

---

## What it is

To sell a subscription on a phone, you go through Apple's **App Store** or Google's **Play Market** (Play Store). They handle the payment — and take a cut. These terms describe how that works.

_The core terms, everyday explanation first:_

| Term | Think of it as... | Precise meaning |
| :--- | :--- | :--- |
| **Commission** | The store's "rent" on every sale | The **% the store keeps** from each subscription. Standard is **30%**. |
| **Small Business Program** | A discount on that rent for newcomers | Apple/Google program that **cuts commission to 15%** for developers under **$1M/year**. |
| **SKU / product** | One specific thing on the shelf | A single purchasable item you define in the store (e.g. "monthly bundle"). |
| **Offer code** | A store-issued coupon | A code Apple/Google generates that gives a **discount or free period** on a subscription. |
| **Auto-renewable subscription** | A gym membership that rebills itself | A subscription the store **charges again automatically** each period until cancelled. |

---

## Why / when to use it

The commission directly shrinks every dollar you earn, so it changes which prices are viable:

_What you actually keep after the store's cut:_

| Price | Standard 30% — you keep | Small Business 15% — you keep | Action needed? |
| :--- | :--- | :--- | :--- |
| $0.99/mo | $0.69 | **$0.84** | Enroll in 15% program |
| $3.99/mo | $2.79 | **$3.39** | — |
| $6.99/mo | $4.89 | **$5.94** | — |

This is why a permanent **$0.99** promo is dangerous: even at the best 15% rate you keep only ~**$0.84**, which barely covers costs. And it is why **enrolling in the Small Business Program** is a must — it nearly doubles what you keep on cheap tiers.

> [!WARNING]
>
> Apple's native **offer codes** have hard limits that break per-influencer tracking:
>
> - Only **10 active custom codes** per subscription product at once.
> - Apple's notifications report the **offer name, not which code** a buyer used.
> - One-time codes **expire after 6 months**.
>
> So you cannot give hundreds of bloggers their own trackable Apple code. Per-influencer attribution must be handled in your own backend (a future technical doc), not by the store.

---

## Example

The same $6.99 subscription, before and after enrolling in the Small Business Program:

```text
$6.99/mo  at 30% commission -> you keep $4.89
$6.99/mo  at 15% commission -> you keep $5.94   (+$1.05 every month, per user)
```

Across hundreds of subscribers that difference is the gap between sustainable and not.

---

## Key points / gotchas

- **The store always takes a cut** — price with the 15% or 30% already subtracted in mind.
- **Enroll in the Small Business Program** before launch; you qualify while under $1M/year.
- **Cheap tiers are punished hardest** by commission in relative terms — a $0.99 plan loses a big slice.
- **Apple offer codes do not scale to many named influencers** — use them only as a single shared discount, never for per-blogger tracking.

---

## Common mistakes

- **Forgetting commission when setting a price** — your real revenue is 70% (or 85%) of the sticker price.
- **Not enrolling in the Small Business Program** and silently giving the store double its cut.
- **Trying to use Apple offer codes per influencer** — the 10-code limit and blind attribution make it impossible at scale.

---

## References

- [Apple Developer — App Store Small Business Program](https://developer.apple.com/app-store/small-business-program/)
- [Apple Developer — Set up subscription offer codes](https://developer.apple.com/help/app-store-connect/manage-subscriptions/set-up-subscription-offer-codes/)
- [Appbot — Apple Offer Codes explained](https://appbot.co/blog/apple-offer-code/)

---

> [!TIP]
> **TL;DR** — The store keeps 30% commission (15% if you enroll in the Small Business Program under $1M/year); a SKU is one purchasable product; Apple offer codes give discounts but cap at 10 active codes and hide which was used, so per-influencer tracking belongs in your own backend.
