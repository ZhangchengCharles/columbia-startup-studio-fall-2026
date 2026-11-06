# SettleWise — Growth Strategy (Nov 9 – Dec 13, 2026)

**Builds on:** `demand_strategy.md` (Oct 22). **Data:** GA4, Oct 9 – Nov 5, 2026 (last 28 days).

## 1. Where we are (GA4 snapshot)

| Signal | Value | What it tells us |
|---|---|---|
| Active / new / returning users | 65 / 67 / 11 | Small base; ~17% come back |
| Avg. engagement / engagement rate | 3m 21s / 44% | People who engage, engage deeply |
| New users by channel | Direct 92%, Social 3 users, Referral 2 | Demand-plan channels aren't showing up; no UTM traffic recorded |
| Top pages (views) | Home 189 · Dashboard 97 · Create account 26 · Log in 22 · StreetEasy listing 15 | Interest exists, but only ~1 in 7 home views reaches signup |
| `form_start` | 13 users (20%) | Intent to sign up is there |
| Key events (signups) | **0** | Signups are not being measured |
| Chrome vs. Safari | 5m 30s vs. **9s** engaged | Possible Safari/iPhone experience problem, or Chrome is inflated by team testing |
| Geography | US 46 users (4m 40s); 10 users from 8 other countries at ~0s | Non-US traffic looks like bots/noise |

**Biggest gaps:** (1) we can't see conversions, (2) we can't credit growth to any channel, (3) Safari users are leaving almost right away.

## 2. Fix the measurement first (by Nov 15)

1. Mark `sign_up` (or the account-created event) as a **key event** in GA4. Confirm it fires on the Create account page.
2. Filter out **internal traffic** (team IPs or a `?internal=1` cookie) so Dashboard and Chrome numbers show real users.
3. Put **UTM links on everything** in the demand plan (social, Reddit, blog, email). Right now that traffic lands in "Direct."
4. Exclude obvious bot countries from reporting, or build a "US only" comparison.

## 3. Growth levers

**A. Fix the signup funnel.** Home → Create account → completed signup is the main leak. Test one change per week: a clearer hero CTA, "try a listing check before signing up" (StreetEasy listing pages already get views), and fewer form fields. Target: 13 form starters → 50% completion.

**B. Fix Safari/mobile.** Test the full flow on iPhone Safari this week. If a bug or layout issue explains the 9s engagement, fixing it could roughly double effective traffic, since a third of users are on Safari.

**C. Make demand channels count.** Focus the demand plan's effort where intent is highest: **r/NYCapartments, r/AskNYC, and Columbia housing channels**, using the StreetEasy-listing check as the hook ("paste a listing, see red flags"). Use social to repurpose winners, not as the main driver until UTMs prove it works.

**D. Retention loop.** 11 returning users is the seed. Send a "your saved listing changed / new red flags" style email or a weekly digest, then measure 7-day return rate.

## 4. Targets and weekly cadence

| By | Goal |
|---|---|
| Nov 15 | Signup key event, internal filter, UTMs live; Safari issue diagnosed |
| Nov 29 | 50+ non-direct (attributed) users; ≥10 completed signups tracked in GA |
| Dec 13 | 150 active users / 28 days; 25+ signups; returning users ≥ 25% |

Every Sunday, add to the demand-plan report: **sessions by UTM source, form_start → sign_up rate, Safari vs. Chrome engagement, returning users.** Double down on the top channel and drop the weakest.

> **Assumptions:** It's unclear how much Chrome/Dashboard traffic is internal, and we don't have real signup counts yet. These targets are estimates and should be recalibrated once Section 2 is in place.
