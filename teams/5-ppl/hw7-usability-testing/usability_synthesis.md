# UnlockDrill: Usability synthesis

**Team:** 5 PPL  
**Product:** UnlockDrill, a web app plus an iPhone Shortcuts automation that shows one SAT question before you open the app you scroll  
**Aha moment:** The user finishes one short practice attempt and understands its explanation, at a moment they would otherwise spend scrolling. A correct answer is not required.  
**Tasks tested:** (1) Create an account, (2) Set up the automation for the app you scroll most, (3) Answer one practice question and read its explanation

## Summary

**Sessions run:** 6 (November 8–13, 2026). Sessions are in [`sessions/`](sessions/).  
**Strangers:** 4 of 6. P2, P3 and P5 were strangers. P6 was a stranger to the moderator and a coworker of another team member. P1 was an acquaintance and P4 a family friend.  
**Recording:** All 6 declined recording; we used written notes only, with a separate moderator and note-taker in every session.

**Participants who reached the aha moment:** 5 of 6, with caveats:

| | P1 | P2 | P3 | P4 | P5 | P6 |
|---|---|---|---|---|---|---|
| Device | iPhone | iPhone | iPhone | iPhone | Android | iPhone |
| Created account | Yes | Yes (after asking why) | Yes | Yes | Yes | No (guest) |
| Finished setup | With help | Yes | Yes | With help | No (Android) | No (gave up) |
| Reached aha | Yes, min 12 | Yes, min 9 | Yes, min 8 | Partly, min 14 | Yes, min 6 (preview only) | No |

- Only **2 of 6** (P2, P3) got through the full intended flow (account, setup, question) **without help**.
- Each of the four who needed help or quit (P1, P4, P5, P6) got stuck or stopped at **setup**.
- Testers who reached the aha moment understood the product right away. P1: "When I got one wrong and it explained the mistake right away." Setup is what stands between people and that moment.

## Patterns across sessions

1. **The file steps in Shortcuts setup stall people. (4 of 6: P1, P3, P4, P6)**
   - P1 left the If action on "File Size" and needed a moderator prompt.
   - P4 lost their place switching between apps and mixed up Text and Save File.
   - P6 stopped at "Delete Files / Delete Immediately" and quit around minute 5.
   - Even P3, who is comfortable with technical instructions, reread the temporary-file explanation.
   - Two magic-wand answers asked for the same fix: "Make setup one button" (P1) and "Give me a finished shortcut instead of making me build it" (P6).
2. **People want to try it before making an account, and the sign-in screen gets in the way. (4 of 6: P1, P2, P5, P6)**
   - P1 landed on "Welcome back" and thought they were on the wrong page.
   - P2 asked, "Can I see what it does before I give you my email?"
   - P6 read Privacy first and chose guest mode.
   - P5 created an account before finding out the main feature didn't work on their phone.
3. **People worry about being forced, locked or annoyed. (3 of 6: P2, P4, P6)**
   - P2 found Skip before reading the question. They asked whether a wrong answer locked TikTok, and said the name made them think they had to "unlock" the app.
   - P2 changed frequency from every open to every third open, and P4 picked once a day because frequent math "sounded stressful."
   - P6 worried about setting something up wrong on their phone.
4. **Explanations and the mistake log matter once people are in. (2 of 6: P3, P4)**
   - P3 tapped the mistake-log entry expecting to reopen the problem.
   - P4 read the explanation twice and still asked why there was a −7 case.
5. **The iPhone requirement is discovered too late. (1 of 6: P5, our only Android tester)**
   - P5 signed up, searched their phone for Shortcuts, and only then found the iPhone-only FAQ at the bottom of `/setup`.

## What surprised us

- The question itself was never the problem. Every tester who reached a question understood what the product was for within seconds of reading the explanation.
- **Guest mode saved P6's account creation, but not P6.** Not having to sign up didn't matter, because setup came before the question and they quit there. They declined to try the preview afterward.
- The fastest aha moment (P5, minute 6) came from **"Preview the question screen"**, a small link hidden inside the setup form, and not from the intended flow.
- P3, our most serious studier, got most excited about the **mistake log**, not the interruption.

## What we're changing and why

Most important first.

> **What we observed:** 4 of 6 testers stalled on the file steps in setup (Get File, If "has any value", Delete Files, Text, Save File). P1 and P4 needed a moderator; P6 quit at minute 5. Two testers independently asked for a ready-made shortcut.
>
> **What we're changing:** Publish a prebuilt "UnlockDrill" shortcut (iCloud share link) that already contains the Get File → If → Delete Files → Stop → Text → Save File → Open URLs logic. On `/setup`, replace the 8 manual steps with 3: (1) tap **Add UnlockDrill Shortcut**, (2) in Automation, choose App → your app → Is Opened → Run Immediately, (3) add the single action **Run Shortcut → UnlockDrill**. Move the current manual steps into a collapsed "Build it yourself" section for people who don't want to import a shortcut. Add a 20-second screen recording next to step 2 (P1 asked for "a short video showing exactly what to tap").
>
> **Why:** Every session that stalled in setup stalled on the file logic, never on picking the app. Once the file logic is prebuilt, users never touch those steps, and P6's question ("which file will be removed?") disappears.

> **What we observed:** 4 of 6 testers hit the account wall before seeing value. P1 thought "Welcome back" meant they were on the wrong page. P2 asked to try before giving an email. P6 went guest. P5 made an account for a feature their phone can't run. Meanwhile, the fastest aha moment came from the hidden preview link.
>
> **What we're changing:** (a) Make **Try a question** the primary button on the homepage and landing pages, and make "Set it up on iPhone" secondary. (b) After the explanation on a demo question, show "Save this to your mistake log: create an account" as the sign-up prompt. (c) Any "Sign up" link opens `SignIn` in create-account mode, so new users never see "Welcome back." (d) On `/setup`, move "Preview the question screen" above the Shortcuts steps as "Try it first."
>
> **Why:** The aha moment is the question and its explanation, and it doesn't need an account or setup. Showing it first means people who get stuck in setup (like P6) have already seen why it's worth finishing.

> **What we observed:** Our Android tester (P5) created an account, then searched for Shortcuts, and only then found "Not yet. It's iPhone only for now" at the bottom of `/setup`. Quote: "I could make an account before realizing the main feature wouldn't work on my phone."
>
> **What we're changing:** Detect non-iOS devices on the homepage, landing pages and `/setup`. Show a banner above the fold: "Automatic questions need an iPhone. On Android you can still practice here. Bookmark this page and we'll email you when Android is ready." Link it to the existing question flow and the update-list signup.
>
> **Why:** Only one session, but it's a hard blocker, it's cheap to fix, and it gets an honest signup from Android users instead of a frustrated one.

> **What we observed:** P2 checked for Skip before reading, asked whether a wrong answer locked the app, and said the name made them think they had to "unlock" their app. P2 and P4 both picked lower frequencies to avoid being annoyed or stressed.
>
> **What we're changing:** On the question screen, add one line under the question: "Skip anytime. Right or wrong, you go straight back to {app}." On `/setup`, move the "Is this an app blocker? No…" answer from the bottom band to sit right under the frequency selector, and make "Every third open" the default instead of "At most once an hour."
>
> **Why:** P2 only relaxed ("Okay, so I don't have to get it right to leave") after finding out for themselves. Saying it up front removes that fear before it costs us a tester.

## What we're not changing (yet)

- **Step-by-step explanations (P4).** Valuable, but it's a content project across every question, and only one tester needed it. We'll log it and look at which explanations people reread once we have analytics on the question screen.
- **Retrying a missed problem from the mistake log, and building a review session from past mistakes (P3).** This is a strong retention idea from our most motivated tester, but it comes after the aha moment, not before it. We'll come back to it after the setup fix ships.
- **Choosing the hours when questions appear (P2).** Shortcuts' Time of Day trigger could support it, but it would add setup steps, which is the opposite of our top fix. We'll revisit after the prebuilt shortcut.
- **An Android automation (P5).** There's no Shortcuts equivalent we can rely on. For now we're only making the limitation visible earlier.
- **Renaming the product (P2's "unlock" confusion).** One tester raised it. We're addressing it with copy first (see change 4).
