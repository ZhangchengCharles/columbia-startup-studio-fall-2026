# Weekly Update: UnlockDrill (5 PPL), November 13, 2026

#### Accountability: what we did

- Build: We didn't ship new features this week. Instead we planned a build sequence for the changes coming out of testing, ordered so each one fixes a real usability problem without breaking the feel of the app (one quick question, then straight back to what you were doing) or drifting from the long-term goal of making practice a habit. This differs from the plan because we wanted usability results before changing the product, so we'd build the right thing first.
- Grow: We reached out through friends and family, and contacted teachers and other people we know who work with SAT students, to get more people trying UnlockDrill. Several of our usability testers came through these connections. This differs from the plan, which centered on blog post 2 and SAT Discord servers: personal outreach was a faster way to reach real SAT takers this week, and it also gave us testers.
- Analyze: Our analysis this week was focused on usability testing rather than site analytics. We went through notes from all 6 sessions, compared where each tester got stuck, and tracked who reached the aha moment and how long it took. This differs from the plan because, before we push more traffic to the site, watching people use the product tells us more than dashboard numbers would.
- Research: Ran 6 usability sessions (Nov 8–13), 4 with strangers, all with SAT takers aged 18–19. 5 of 6 reached the aha moment, but only 2 of 6 got through account, setup and first question without help. Every tester who stalled or quit (4 of 6) did so during Shortcuts setup, mostly at the file steps (Get File, If, Delete Files, Save File). One Android tester signed up before learning the automation is iPhone-only. See `hw7-usability-testing/usability_synthesis.md`.

#### Planning: what we're doing next

- Build: Ship a prebuilt UnlockDrill shortcut so `/setup` drops from 8 manual steps to 3 (add shortcut, create the App automation, Run Shortcut). Setup was where every stalled session got stuck, and two testers asked for exactly this. Next: make "Try a question" the primary homepage button and ask for an account after the first explanation, because 4 of 6 testers hesitated at sign-up before seeing value.
- Grow: Follow the demand plan for the week of Nov 16 (owner: Linfeng Li): an AMA-style post on what we learned from interviews and usability tests. Send traffic to "Try a question" instead of setup, so visitors hit the aha moment first.
- Analyze: Set up a GA funnel: visit → demo question answered → account created → setup completed. This tells us whether the prebuilt shortcut and try-first flow actually raise setup completion.
- Research: Re-run 3 usability sessions with strangers on the new setup, including at least one person who has never used Shortcuts. We need to see whether people finish setup without help.

#### Issues

- The automation is iPhone-only. Android users can practice in the browser but can't get the interruption, which limits part of our audience.
- All 6 testers declined recording, so we only have written notes to review.
