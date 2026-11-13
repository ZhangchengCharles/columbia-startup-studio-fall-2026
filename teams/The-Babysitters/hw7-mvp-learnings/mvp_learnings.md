# Homework 7 — MVP learnings

**The Babysitters · Claude Daycare**
Mitchell Rosenthal, Almog Ankori, Josh Hegstad, Mansi Rank

## What the midterm feedback told us

Two things came back at us after the midterm. People were nervous about what our agent could reach on their computer, and people didn't want to spend their own paid AI allowance on a visit. For a couple of weeks I treated those as two separate complaints with two separate fixes, one about sandboxing and one about pricing.

I don't think that's right anymore. Both are the same question asked twice, which is what the owner actually gets for sending their agent out. Someone who can see a real payoff tolerates a real cost and reads a permission prompt carefully. Someone who can't see the payoff isn't negotiating about either one, they're declining politely. That reframing is the main thing we learned this cycle, and it ruled out the obvious response, which would have been to add a sixth activity to the list and hope one of them landed.

## What we're changing

Claude Daycare becomes a place agents compete rather than a place they play.

Several challenges run at the same time. An owner sends their agent with as much or as little direction as they want. The agent enters on its own, works against a published brief, and submits a result. The result gets scored on the brief's stated goals plus real preference from people on the site, using a 40% human preference, 40% goal completion, 20% accessibility rubric for the design example. The winning approach then becomes a reusable skill in a platform library, and other owners can unlock it for their own work with credits they've earned or bought.

The reason to come back is a skill that helps with the owner's real work. An interesting result, something learned, or a better sense of what these tools can actually do all count as secondary payoffs, and a visit can be worth it on those alone.

## The decisions that follow from it

Five questions we'd been leaving open got settled, and each one changes what we build.

A skill is local text files, instructions plus worked examples, the same shape as any other skill an agent loads. Using one inside a challenge works on trust. Spending credits is what lets an owner keep a copy.

An agent can carry its owner's memory in, but only after walking through it with the owner item by item, from the first version rather than bolted on later. A question the owner never answered does not count as a yes.

The agent works on the owner's own machine with the owner's own tools, then uploads the result. Per-challenge folder scoping and spending caps are the next decisions underneath this one.

Anyone with an account can vote, picking a favorite from the full list of entries.

A winning skill's usefulness gets checked by handing it to a fresh agent on a new brief, several runs with it and several without, on the same budget, with the comparison published on that skill's page.

## What we cut on purpose

The first version has no collaboration at all. Solo entries, no teams, no agents recruiting other agents.

That one cost us something real, because wanting to watch agents talk to each other is the idea this whole project started from. We gave it up for now because a competition between independent entries can actually be judged, and a collaboration can't be, not yet. We don't have a way to tell which agent in a group did the work, and inventing an individual hero score inside a cooperative game would be making up a number.

Rewards are set per game rather than by one formula across the platform, so a design challenge and a spreadsheet repair can pay differently without us pretending they're equivalent. And the skill library belongs to the platform rather than to whoever won it, which rules out a version we'd considered where winners would list and price their own skills.

## What our own code actually supports today

We inspected the platform repo read-only against the new direction instead of assuming our existing features would carry over. The honest summary:

What's there: activity discovery, joining, seats, configurable rules, recorded moves, and a turn engine that validates legal turns against round and move limits. Tycoon runs one visitor against two model-simulated companies and ranks closing valuation. Daily Question, paper trading, essays, chat, DMs and friends exist. Daycare memory can be saved and listed per actor.

What isn't there: any submission, judging, scoring, or reward machinery for artifacts. The turn engine validates moves, it doesn't evaluate whether a thing someone made is good. There's no skill library at all, no submission, search, versioning, provenance, reuse, or evaluation. The existing paper-trading credits don't generalize into the skill economy we've described. And the documented runner turns have no file or shell access, which matters below.

Finding that out early is worth more than it sounds. It means the lifecycle is the build, not a feature on top of a working platform.

## Open risks we've named

Three things concern me, and I'd rather have them written down than discover them in December.

Our execution decision argues against our own safety story. The runner today launches the agent into a throwaway workspace with no file, shell, or browser access, and our trust page describes exactly that isolation as the reason to trust us. It's also what I pointed at in October every time somebody raised security. We've now decided agents should work on the owner's real machine with their real tools, which is a far more useful product and a much bigger surface to worry about. We haven't yet decided what promise replaces the one we're giving up, and rewriting both the launch and the trust page is on this week's list.

Competing costs more allowance than visiting did, not less. The skill transfer tests cost more again. The complaint was that a visit wasn't worth the tokens, and our answer raises the bill and bets the payoff is now obviously worth it. That's a bet, and it's the specific thing our sessions are built to test.

Challenge-only skill access is a rule and not a mechanism. If we hand an owner's local agent the full text of a skill, that owner can keep it. Writing "challenge use only" into the rules doesn't stop a copy. Before we build a credit ledger I want to know whether a credit buys a file, a permission, or just a convenience, because the three have different products behind them.

## How we're testing what's left

Two assumptions hold up the whole direction and neither has evidence yet. Would an owner spend their own paid allowance to enter a competition, and would they rather have the winning method or the thing the winner actually made.

We wrote a moderated usability script for both, in `usability_test_script.md` in this folder. Twenty to twenty-five minutes, run with strangers rather than friends, recorded with consent. Six parts: what the participant actually uses today, unaided comprehension of the homepage, a printed challenge brief, the reward and the two-currency system, memory approval and the disclosure that the agent runs on their machine, then whether they'd return and what would have to have happened first.

A few choices in it are deliberate. We don't explain the product during a session, because if someone can't work out what it is from the page, that's the finding. We ask what people would do rather than whether they like something. Part 1 asks whether they've ever actually hit a usage limit before we show them anything, because if nobody has, our framing is a guess and we need to know that. And the note sheet has a row for contrary evidence, since our October feedback was useful precisely because it was negative.

Results get reported as raw counts across participants with a blocker, major, minor, or cosmetic severity rating, never as percentages. Five sessions give counts, not rates.

## What we'll know by next Friday

Whether a stranger can say what this is without help, whether anyone would spend their allowance on it and under what condition, whether the skill or the artifact is the thing they want, and whether running on their own machine reads as useful or as a reason to stop. Plus one complete challenge round that can open, take a solo entry, close, get judged by people, and finish.

That's a narrower list than we'd have written a month ago. It's also the first version of this product where I can answer why somebody would send their agent a second time, which is the question we'd been failing since the midterm. The work now is to close the trust gap we opened, test the cost assumption with real people, and settle what a credit buys before it turns into a database schema.
