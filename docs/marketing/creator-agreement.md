# Creator Agreement: Example, Signing, and Going Without

`marketing` · `influencers` · `legal` · `operations` · **Level:** Intermediate

> [!NOTE]
> An example one-page barter agreement, the practical ways a creator actually signs it, and an honest look at what happens if you proceed without one.

---

## What it is

The agreement layer of the [outreach playbook](creator-outreach-and-barter-ops.md). For a nano/micro barter deal — free lifetime premium plus a personal promo code and a revenue share — you do **not** need a long legal contract. You need a **one-page plain-language agreement** that pins down the deal and carries the legally required `#ad` disclosure clause. This doc gives an example of that page, three realistic ways to get it signed, and the real consequences of skipping it.

> [!IMPORTANT]
> This is **not legal advice.** The example below is a starting point to adapt and have a lawyer review before real use. FTC rules are US law; for a globally available app, see [disclosure-rules-by-country.md](disclosure-rules-by-country.md) for the UK, EU, Canada, Australia, and other markets — the same `#ad` clause covers nearly all of them.

---

## Why / when to use it

Because the everyday failure in barter is not a lawsuit — it is a creator who takes the free premium and never posts, or posts something off-brand. The data backs this: **67%** of influencer–brand disputes come from **unclear terms, not actual performance failures**. A one-page agreement removes that ambiguity for almost no cost, and at the same time carries the FTC clause that caps your legal exposure.

> [!IMPORTANT]
> For a small brand operating internationally (e.g. based in Ukraine, creators abroad), the agreement is **not** a tool to punish creators in court — cross-border lawsuits are not viable, and small-claims courts do not work across borders. Its real jobs are **liability-shifting** (the `#ad` clause moves disclosure liability onto the creator), **setting expectations**, and a **paper trail**. Your actual enforcement is the **backend kill-switch** below.

---

## Backend enforcement (your real lever)

The agreement documents the deal; your **server** enforces it. Because everything you give a creator is **ongoing and revocable**, you never need a court.

_What you control directly, instantly, for free:_

| Creator behaviour | Your response from the backend |
| :--- | :--- |
| Does not post | **Deactivate their promo code; revoke free premium** |
| Posts without `#ad` | Same — pause until fixed |
| Drives chargebacks / fraud via their code | Kill the code, stop revenue share |
| Honours the deal | Keep everything active; pay the share |

This is **self-help enforcement**: you paid no cash up front, so there is nothing to claw back — you simply stop giving. For barter, this beats a contract because the leverage is structural, not legal.

> [!WARNING]
> Do not pay a lawyer expecting to chase creators across borders. The proper cross-border tool (international arbitration under the New York Convention) is built for deals worth tens of thousands, not a free app subscription. Design the system so the kill-switch is all you ever need.

---

## Example

A fill-in-the-blanks one-page agreement. Replace every bracket; keep the structure short on purpose.

```text
CREATOR PARTNERSHIP AGREEMENT (Barter)

Between: [Your business name], "the Brand" ([email])
And:     [Creator full name / handle], "the Creator" ([email])
Date:    [date]

1. What the Creator does
   - Publishes [N] post(s) / [N] story(ies) about [App] on [platform(s)]
     between [start date] and [end date].
   - Each post clearly discloses the partnership using #ad or #sponsored,
     placed where it is easy to see (per FTC Endorsement Guides).
   - Does not make claims about [App] that are untrue or unproven.

2. What the Brand gives
   - Free lifetime premium access to [App] (and: [list other apps]).
   - A personal promo code ("[CODE]") giving the Creator's audience
     [discount] for [intro period].
   - [X]% of the net subscription revenue generated through [CODE],
     paid [monthly] via [method], starting [when].

3. Content and approval
   - The Brand may review a post before publication and request changes
     to factual accuracy or disclosure only.
   - The Creator keeps ownership of the content; the Brand may reshare it
     with credit.

4. Disclosure responsibility
   - The Creator is responsible for complying with FTC disclosure rules.
   - The Brand will never ask the Creator to hide or remove the #ad label.

5. Ending it
   - Either side may end this with [7] days' written notice.
   - The promo code is deactivated when the agreement ends; revenue share
     is paid out for sales made before that date.

Agreed:
Creator: ______________________  Date: __________
Brand:   ______________________  Date: __________
```

---

## Key points / gotchas

How they actually sign it — three realistic options, cheapest and simplest first:

_Ways to get the agreement signed:_

| Method | How it works | Best when | Effort |
| :--- | :--- | :--- | :--- |
| **Free e-signature tool** | Upload the page as a reusable template, send a link, they sign in-browser. OpenSign (unlimited free), DocuSeal (open-source / 10 free per month), Dropbox Sign or Xodo Sign (3 per month free). | Your scale (~80 creators) — proper signatures, a stored record | Low, one-time setup |
| **Google Form as agreement + consent** | The form states the terms; a required "I agree" checkbox plus their name/email is the assent. Doubles as your tracking sheet. | Very lightweight barter, fast onboarding | Lowest |
| **Email confirmation** | Paste the terms, they reply "I agree." | A quick paper trail when nothing else is set up | Lowest, weakest |

- **Use a reusable template.** Set the one-pager up once in DocuSeal or OpenSign and reuse it for every creator; do not rewrite per person.
- **A checkbox/email "I agree" is real assent** for low-stakes barter — it is a record, not a handshake — but a true e-signature is stronger if a deal ever goes sideways.
- **The agreement and your tracking sheet can be the same Google Form**, which removes a step.

---

## Is a Google Form valid proof — and does asking them to disclose protect me?

Two separate questions, two different answers.

_Is a Google Form valid consent across countries?_

| Jurisdiction | A checkbox "I agree" is... | Catch |
| :--- | :--- | :--- |
| **US** (ESIGN/UETA) | A valid e-signature if it shows intent and is tied to the person | Courts have upheld checkboxes |
| **EU** (eIDAS) | A valid **simple** electronic signature | The **weakest** evidentiary tier (below advanced/qualified) |
| **Most others** | Generally valid for low-stakes agreements | Same — it is the floor, not strong proof |

> [!IMPORTANT]
> A bare Google Form response is **weak evidence on its own**. To be defensible it needs clear consent language, **identity metadata (email, IP, timestamp)**, and an **unaltered record** of what was agreed. A proper e-sign tool (DocuSeal/OpenSign) captures that automatically, which is why it is stronger for the same effort. For low-stakes barter a Form is acceptable; do not rely on it for anything bigger.

_Does proof that you asked them to add `#ad` protect you from regulators?_

> [!WARNING]
> **No — "I instructed them" is not a complete defense.** The FTC requires brands to do three things: **instruct** (exact wording + placement), **monitor** what they actually post, and **take corrective action** when they do not. The signed Form proves only the first. If a creator forgets `#ad` and you did nothing, you are **still liable**.

The useful part: steps 2 and 3 are exactly your **backend kill-switch** — check that the creator actually posted with `#ad` (you track their code anyway), and deactivate the code or pause premium if they did not. So the same kill-switch that enforces the deal **is also your FTC compliance mechanism**. The Form proves the instruction; the kill-switch proves the monitoring and correction.

---

## Common mistakes

What happens if you proceed without any agreement — the honest version:

_Risk of going without, by type:_

| Risk type | What actually happens | Severity |
| :--- | :--- | :--- |
| **Operational** | Creator takes free premium and never posts, posts late, or posts off-brand; "scope creep" — they expected more than you did | High, and common |
| **Legal (FTC)** | No clause forces `#ad`; if the Creator does not disclose, the **Brand shares liability up to $53,088 per violation** | Lower odds, severe |
| **Ownership / expectations** | Nothing written means disputes over what was promised; you also cannot reuse their content. (Note: enforcement is the **backend kill-switch**, not the courts — see above) | Medium |

- **Going without is survivable for one tiny barter deal** — many people do it — but it **scales badly**. At ~80 creators, "a few ghost you, one triggers an FTC issue" shifts from hypothetical to likely.
- **The cheap fix beats the cheap shortcut.** A free e-sign template costs nothing and removes the two failure modes (no-show and FTC exposure) that actually bite at scale.
- **Skipping the disclosure clause is the one shortcut never worth taking** — it is the difference between the Creator's mistake and your shared liability.

---

## References

- [Zapier — Best DocuSign alternatives 2026](https://zapier.com/blog/docusign-alternatives/)
- [esign.ai — Free DocuSign alternatives](https://www.esign.ai/blog/best-free-docusign-alternatives-individuals-usa-unlimited)
- [InfluenceFlow — Influencer marketing contracts guide 2025](https://influenceflow.io/resources/influencer-marketing-contracts-the-complete-2025-guide-for-brands-and-creators/)
- [FTC — Endorsements, Influencers, and Reviews](https://www.ftc.gov/business-guidance/advertising-marketing/endorsements-influencers-reviews)
- [PAIL Solicitors — Cross-border influencer marketing legal guide](https://pailsolicitors.co.uk/media-solicitors/mastering-cross-border-influencer-marketing-a-legal-guide)
- [esign.ai — Is a checkbox a legal signature?](https://www.esign.ai/blog/is-checkbox-legal-signature)
- [Honigman — Avoiding FTC penalties for brand partners](https://www.honigman.com/the-matrix/mitigating-risk-in-the-influencer-economy-a-legal-guide-to-avoiding-ftc-penalties-for-brand-partners)

---

> [!TIP]
> **TL;DR** — Use a one-page plain-language barter agreement for liability-shifting and clear expectations (not for suing anyone — cross-border lawsuits are not viable from Ukraine); a Google Form checkbox is valid-but-weak consent in most countries (an e-sign tool is stronger for the same effort), and proving you "asked for #ad" is **not** a complete regulator defense — you must also monitor and correct, which is exactly what your **backend kill-switch** does, so the same kill-switch is both your enforcement and your FTC compliance.
