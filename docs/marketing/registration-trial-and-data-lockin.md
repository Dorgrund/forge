# Local Trial, Then Combined Register-and-Subscribe Gate

`marketing` · `pricing` · `trial` · `retention` · `ux` · **Level:** Intermediate

> [!NOTE]
> A 3-day fully anonymous local trial followed by a single Day-3 gate that creates the account and starts the subscription together, with the trial-reset loophole and how to handle it.

---

## What it is

The simplest staged design, made stronger by an **offline-first, cloud-sync** architecture: the user runs the app **anonymously on local storage for 3 days** with no signup, and on **Day 3 hits one gate** that does **register and subscribe at the same time**. There is no Day-1 interruption — a clean 3-day experience, then a single decision. Creating the account **syncs the local data to the cloud** under that account, so the 3 days of history carry over and become server-backed.

_The two phases:_

| Phase | What happens | Where data lives |
| :--- | :--- | :--- |
| **Day 0–3** | Full anonymous use, no account, app works fully offline | **Local storage** on the device |
| **Day 3 gate** | One screen: create account **and** subscribe | Local data **syncs to the cloud** under the new account |

---

## Why / when to use it

This is gentler and simpler than a separate Day-1 register gate, with one accepted trade-off.

- **One interruption, not two.** Users get an uninterrupted 3-day run, then a single ask at the moment motivation is highest — early/onboarding placement is where **~50%+ of trial starts** happen.
- **Simpler to build.** Local storage for the trial, no anonymous-auth backend, no Day-1 upgrade flow; the account is created once, at purchase.
- **Apple-safe.** Registration is asked **at the point of purchase** (the account is genuinely needed to attach the subscription), so there is no Guideline 5.1.1 "forced registration before use" problem.

> [!IMPORTANT]
> The loophole is **narrow** here because the apps are offline-first with cloud sync. Only the **pre-account days (0–3)** are local-only, so a determined user could clear local storage and reinstall for another fresh 3 days. But the moment they convert, their data **syncs to the cloud under an account**, giving you a **server-side identity** — so a reinstall then **restores** their data (good for honest users) and your backend **recognises the returning account** (bad for farmers). The reset loophole exists only before first conversion, not after.

---

## Example

The flow, with the data migration that keeps subscribing rewarding.

```text
Onboarding (screen 1-2):
  "Try [App] free for 3 days. On day 3, create an account and
   subscribe to keep going — your data comes with you."

Day 0-3 -> full anonymous OFFLINE use; everything saved to LOCAL storage
Day 3   -> ONE gate: "Create your account and subscribe to continue"
           - account created
           - subscription started
           - local data SYNCS to the cloud under the account
             (history preserved AND now server-backed)
```

_Where the loophole does and does not apply, given offline-first + cloud sync:_

| Window | Trial-reset possible? | Why |
| :--- | :--- | :--- |
| **Before first account (Day 0–3)** | Yes, by clearing local storage / reinstalling | No server-side identity yet |
| **After conversion** | No | Data is in the cloud under an account; reinstall **restores** it and the backend **knows** the account |

_Handling the remaining pre-account window if farming becomes real:_

| Concern | Reality | Optional mitigation (add later) |
| :--- | :--- | :--- |
| Reinstall to reset the first 3 days | A small minority bother; most find it too annoying | Device-level signal (`identifierForVendor`) or a privacy-respecting receipt check — **without** forcing a Day-1 account |

Optimise for the ~95% who will not farm; the cloud sync already closes the loophole the moment they convert.

---

## Key points / gotchas

- **Asking for the account at purchase is the most legitimate moment** — Apple 5.1.1 is satisfied because the account is needed for the subscription.
- **Sync local data to the cloud at the gate** so subscribing preserves the 3 days and makes the history server-backed — keep the "your data comes with you" incentive without a Day-1 lock-in.
- **Cloud sync closes the loophole at conversion.** The reset trick only works in the pre-account window (Day 0–3); once synced, the account is a server-side identity a reinstall cannot wipe.
- **Announce the 3-day terms in onboarding.** Up-front disclosure is what keeps it honest rather than a surprise (see [hard-paywall-transparency.md](hard-paywall-transparency.md)).
- **Offer Sign in with Apple** if the combined gate uses any social login.
- **Be exact about "3 days"** — define 72h-from-first-open vs calendar days and show it consistently.

---

## Common mistakes

- **Not syncing local data to the cloud at the gate** — subscribing then feels like starting over, killing the incentive to convert.
- **Forgetting the pre-account window is still local** — the reset trick works until first conversion, so add a device signal there if farming becomes real; do not assume the Day 0–3 local state is tamper-proof.
- **Over-engineering anti-abuse on day one** — the farming minority is small; heavy friction costs more conversions than it saves.
- **Hiding the 3-day limit** until the gate appears — produces the surprise-driven anger this design should avoid.
- **Social login without Sign in with Apple** — violates Apple's rules.

---

## References

- [retention.blog — Onboarding doesn't end at the paywall](https://www.retention.blog/p/onboarding-doesnt-end-at-the-paywall)
- [vmobify — App onboarding best practices](https://vmobify.com/blog/app-onboarding-best-practices)
- [RevenueCat — Essential guide to mobile paywalls](https://www.revenuecat.com/blog/growth/guide-to-mobile-paywalls-subscription-apps/)
- [Apple Developer Forums — Clarification on Guideline 5.1.1(v)](https://developer.apple.com/forums/thread/724336)

---

> [!TIP]
> **TL;DR** — Run a 3-day fully anonymous offline local trial, then a single Day-3 gate that creates the account and starts the subscription together, syncing the local data to the cloud so history is kept and becomes server-backed; it is simpler and Apple-safe because registration happens at purchase, and because the apps are offline-first with cloud sync the reset loophole only exists before first conversion — after that the cloud account is an identity a reinstall cannot wipe.
