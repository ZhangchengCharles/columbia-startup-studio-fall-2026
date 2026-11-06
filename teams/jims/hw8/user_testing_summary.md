# SettleWise — Usability Testing Write-up (HW 8)

**Sessions:** 5 first-time users, Nov 5–6, 2026 · ~20–24 min each
**Hosts / note-takers:** Maria (P1), Izum (P2, P3), Sami (P4, P5)
**Method:** Think-aloud usability test using the class script (Class 8). Screen recorded and transcribed with consent; findings shared anonymously. Participants are referred to by ID only.

**Aha moment we tested for:** the user realizes SettleWise compares the apartments *they already found*, side by side, based on *their* priorities.

| ID | Host | Sources reviewed |
|----|------|------------------|
| P1 | Maria | Session notes, Zoom transcript, screen recording |
| P2 | Izum | Session notes |
| P3 | Izum | Session notes |
| P4 | Sami | Script notes (Test_User_3), session video + Drive transcript, screen recording |
| P5 | Sami | Observer notes (second note set in the same doc) |

> P5's notes sit in the same doc as P4's but describe different behavior (e.g. used the URL instead of the button), so they're treated as a separate session with notes only.

---

## 1. Tasks

1. **First impressions:** "Open SettleWise. Without clicking, what do you think this does?"
2. **Sign up.**
3. **Add listings:** "Go to StreetEasy, find 3 apartments you'd consider, add all 3 to SettleWise."
4. **Compare (aha task):** "Select at least 3 priorities, then generate a comparison of your 3 apartments."

Post-session questions: when did you get it, most confusing part, what would make it easier, would you use it again, one magic-wand change.

## 2. Results at a glance

| | P1 | P2 | P3 | P4 | P5 |
|---|---|---|---|---|---|
| Understood purpose from landing page | Partial | No | Partial | Yes | No |
| Completed signup | Yes | Yes | Yes | Yes | Yes |
| Tutorial | Skipped | Skipped | Completed | Used | — |
| Added 3 listings | Yes (with help) | Partial | Partial | Struggled | No (nothing saved) |
| Selected 3+ priorities | Not verified | Yes | Yes | Yes | Yes, unsure it worked |
| Generated comparison | Yes | Yes | Yes | Yes | Yes |
| **Reached aha moment** | **Yes** | **Yes** | **No** | **No** | **Partial** |

**2 of 5 clearly reached the aha moment, and both only on the final comparison screen.** Everyone signed up. Every session hit trouble at the same two steps: the add-listing button and the comparison setup.

## 3. What we observed (behavior)

### Landing page and first impression
- 3 of 5 misread the product. P2 thought it was an apartment marketplace and kept that belief until the comparison loaded. P1 thought it was for finding or saving apartments. P5 guessed it was a bill-splitting app because the name reminded him of Splitwise. P2 brought up the Splitwise name too.
- P2 said the page had "so much going on" and gave no clear place to start.
- P3 and P4 picked up apartment search/comparison. P4 first said "a website where I can search for apartments," praised the animations, then added that being able to compare apartments at the same time was "pretty useful."

### Signup and onboarding
- Signup worked for everyone. P4 finished it very quickly.
- P1 and P2 skipped the tutorial. Afterward neither knew what to do next. P2 said he "did not know where to go first."
- After signing up, P5 clicked back to the homepage and got confused that he had to hit "Get started" again (no profile or home base).
- P5 went to StreetEasy before he'd made a search group, then didn't know where his listings should go.

### Adding listings (biggest blocker)
- **The button failed in every session.**
  - P1 asked out loud "What is a bookmark?" and saved it under All Bookmarks instead of the bookmarks bar, so she dug through menus for every listing. Once shown the bookmarks-bar method afterward, she said it was "better."
  - P2 had trouble finding the button and didn't understand how to use it. Once his first add worked, he called the rest easy.
  - P3 struggled with it **even after doing the tutorial**, asked several times for a video showing how it works, and got visibly annoyed switching tabs between SettleWise and StreetEasy.
  - P4 dragged the button onto the tabs instead of the bookmarks bar ("dragging into my... no, I'm not able to"), skipped the instructions, opened the comparison page and found 0 apartments, asked "Drop it to bookmarks? How do I do that?", and only then slowed down to read. Afterward he said the bookmark setup "is a bit confusing" and suggested a **browser extension** instead.
  - P5 never noticed the button and pasted URLs instead. Nothing was pulled in (URL import wasn't working), so he couldn't tell whether anything had saved.
- 3 users (P2, P3, P5) expected **one click to add the listing**, with no extra steps.
- P5: fine with 3 listings, but "if he had 10 properties he would not do it."
- P4 searched in and around Harlem at $1,500 and remarked on how few listings came up. P5 said StreetEasy was overwhelming.

### Comparison setup and results
- **Edit Comparison Fields confused people.** P1 didn't know what "non-negotiables" meant. She read "3 of 3" next to a field as "three bedrooms" when it means "3 of 3 listings have this info." P5 asked why a field said "0 out of 3."
- P1 didn't realize that reordering priorities is a separate step from setting non-negotiables ("I thought it was the same as this").
- P2 and P3 both expected the comparison right after clicking Compare, but hit another page first. P3 "navigated blindly" until the priorities screen.
- P5 clicked priorities without knowing whether they'd do anything. He also disliked setting priorities *before* seeing any comparison: he wanted a default comparison first that he could adjust.
- **What made it click:** P1 when the comparison flagged an apartment over her rent limit. P2 when he saw **net effective rent**.
- P4 generated the comparison but reacted very little ("didn't seem to care... knew what to expect"). In the interview he said that between two of his apartments he didn't "see much of a difference apart from price." The host left asking whether a table alone delivers enough value.

### Post-session answers
- **When did you get it?** P1 and P2: only at the comparison. P3: during the tutorial. P4: the homepage, though how it worked only made sense in the tutorial. P5: from the images, once he saw them.
- **Would you use it again?** P1: yes, if apartment hunting (she usually searches on her phone). P2 and P3: "yes, if I knew what it was for from the start." P4: "Yeah, I would use this... it's a very good idea as a product," but as an extension, because the bookmark step is confusing.
- **Magic wand:**
  - P1: split comparison settings into smaller steps with a Next button
  - P2: less text, a simpler experience
  - P3: no switching back and forth to StreetEasy; listings already inside SettleWise
  - P4: pull in more detail per listing, like "a Google review but for each of the properties" from past tenants, because the current fields don't separate listings beyond price
  - P5: a single "add property" button

## 4. Key findings (ranked)

1. **The add-listing button is the activation killer.** 5/5 struggled; the tutorial didn't fix it (P3). Users expect one click that confirms the add, and P4 suggested a browser extension.
2. **The landing page doesn't say "compare."** 3/5 thought it was a marketplace, a saving tool, or a payment splitter. The Splitwise name association came up twice.
3. **Too many steps and too much text between listings and results.** Extra page before results, a dense Edit Comparison Fields screen, unclear "non-negotiables" and "X of 3" labels.
4. **The comparison output works when it's personal.** Both aha moments came from personal signals: over-budget rent, net effective rent. A generic table didn't land for P4, who saw no difference "apart from price" and asked for richer data like tenant reviews.
5. **Users want the product to do the work first.** Show a default comparison, then let them customize (P5). Ask for less upfront effort (P2, P3).
6. **Onboarding is skippable and post-signup has no home base.** 2 users skipped the tutorial and were then lost. P5 wanted a profile page.

## 5. What we're changing and why

| Change | Why (evidence) | Status |
|---|---|---|
| Remove URL paste; make the button the single, obvious add path | P5 used the URL and nothing saved; P4 and P2 couldn't find the button | **Done** |
| Add "Add apartment" directly on the comparison screen | P4 reached the comparison with 0 apartments and had to backtrack | **Done** |
| Default comparison on base rent shown immediately; priorities layered on after | P5 wanted results before setup; P2 and P3 expected results right after clicking | **Done** |
| New tutorial with a short **video/GIF of the button on a StreetEasy listing** | P3 asked for video repeatedly; P1 and P4 didn't know where the bookmarks bar was | In progress |
| Rewrite homepage headline: "Compare the apartments you've already found, ranked by what matters to you" | P2, P1, P5 misread the purpose | Next |
| Break Edit Comparison Fields into steps (Non-negotiables → Priorities → Results) with a Next button and plain-language labels ("3 of 3 listings include this") | P1's magic wand; P1 and P5 misread the counts | Next |
| Surface personal callouts (net effective rent, over-budget flags) at the top of results | These triggered both aha moments | Next |
| Explore AI-generated recommendation ("Your best fit is X because...") and richer listing data (e.g. past-tenant reviews) | P4 showed no reaction to a plain table and saw no difference beyond price | Exploring |
| Evaluate a browser extension as an alternative to the bookmarklet | P4 suggested it directly; the bookmark step blocked all 5 users | Exploring |
| Add a profile/home page after signup | P5 got lost after signup | Backlog |
| Longer term: reduce tab-switching (SettleWise on StreetEasy, or listings pulled in) | P3's biggest frustration; P5 wouldn't do 10 listings | Backlog |

## 6. Next round of testing

- **Recruit strangers, and don't step in.** Hosts sometimes clarified tasks or explained features mid-session (P1, P5). Per the class guidance, tasks finished with help aren't proof users would get there alone.
- **Give a realistic scenario** instead of "add any 3 apartments": *"You're moving to NYC soon on a budget. Think about what matters most (rent, location, bedrooms, laundry). Find 3 apartments you'd seriously consider, add them, and use the comparison to pick one."* This tests whether SettleWise actually helps someone decide, not just whether they can finish the steps.
- **Hosts don't help.** If stuck, ask only "What are you looking for?"
- **Measure:** time to first listing added, number of failed add attempts, and whether the aha moment happens *before* the final screen.
