# Usability test script

**The Babysitters · Claude Daycare**

Moderated session script for 3–5 participants, strangers rather than friends, recorded with consent. Written for the challenge-and-skill-library direction described in `mvp_learnings.md`. Target length is 20–25 minutes per session.

This script tests comprehension and reaction. It does not establish demand. A participant who likes the idea is not a customer, and an enthusiastic answer to a hypothetical is not evidence that a problem exists.

## What to prepare before the first session

Four stimuli. None of them needs new code.

1. **The homepage** as currently built. Use the deployed page if the public route is verified, otherwise the local build. Record which one was used in every session.
2. **One challenge brief card**, printed or on screen, one page. It must show the brief, what the agent has to produce, the published goals, the 40/40/20 rubric, the reward, and the spending limit.
3. **One winning skill page**, mocked. Show the skill as what it actually is: written instructions plus worked examples, with its provenance and the credit cost to unlock it for personal use.
4. **One memory approval screen**, mocked. A short list of the kinds of things an agent might carry in, each with an approve or decline control.

Label every mock as a concept beside its name. If a participant asks whether something works today, answer honestly and write down that they asked.

## Recruiting

Approach strangers where the relevant behavior happens: Butler and Uris, the engineering building, a campus AI or coding club, a coffee shop near campus. No roommates, no teammates, no friends.

Aim for at least three participants who currently pay for an AI tool. One or two who don't pay is useful rather than wasted, because the install and allowance requirements are a real part of the funnel. Record each participant's actual situation instead of screening toward a preferred answer.

Recruiting line:

> I'm a Columbia student doing user testing for a class project. It's about twenty minutes, I'll ask you to look at a website and tell me what you think it does. I'm not selling anything and there's no right answer. Would you be willing?

## Consent

Read this before recording starts, then start the recording and confirm on tape.

> Before we start: I'd like to record audio and my screen so I don't have to take notes while you talk. The recording is only for my class project. I won't publish your name, and I won't quote you anywhere without asking you first. You can stop at any time, skip any question, and ask me to delete the recording afterward. Is recording okay with you?

Wait for a clear yes. If the answer is no, run the session with written notes instead and record that there's no recording for that participant.

Then:

> One more thing. I'm testing the product, not you. If something is confusing, that's information I need. Please think out loud as you go, including when you're stuck or annoyed.

## Moderator rules

- Don't explain the product. If a participant can't work out what it is, that's the finding.
- Don't rescue. When someone stalls, wait, then ask what they're looking for.
- Don't defend a design or correct a wrong impression until the session is over.
- Never ask whether they like something. Ask what they'd do, and what they expect to happen.
- Record how long comprehension takes and how many times they ask for help.
- Keep your own enthusiasm off the tape. Nodding at the answers you want is how a session turns into a sales pitch.

## Part 1 — Background (3 minutes)

Ground the session in what they actually do before showing anything.

1. What do you use AI for, if anything? Which tools?
2. Walk me through the last time you used one. What were you trying to get done?
3. Do you pay for any of them? Which plan?
4. Have you ever hit a usage limit or had to stop because you ran out? What happened?

Question 4 matters most. The answer either supports or undermines the allowance problem this product is built around. Write down what they say even when it contradicts the premise.

## Part 2 — Homepage comprehension (5 minutes)

Open the homepage. Let them look without saying anything.

> Take as long as you want to read this. Tell me what you're thinking as you go.

When they stop reading, ask these in order, without helping:

5. In your own words, what does this do?
6. Who do you think it's for?
7. If you used it, what would you get back?
8. What do you think that button does?

Then:

9. What would it cost you to use this?
10. Is there anything here you don't believe, or that you'd want to check first?
11. What's the first question you'd want answered that this page doesn't answer?

**Record:** time from first look to a correct answer on question 5, whether they got there at all, and the exact words they used for the product. Their wording is more useful than our headline.

## Part 3 — The challenge (5 minutes)

Hand them the challenge brief card.

> This is one of the activities. Read it and tell me what's going on.

12. What's being asked for here, and who does the work?
13. Say you did this. What would you put in, and what would you get out?
14. How is the winner decided?
15. Does the way it's judged seem fair to you? Why or why not?

Then the question that matters most:

16. Doing this uses part of your own paid AI allowance. Knowing that, would you enter? What would have to be true for you to say yes?

Don't soften question 16 and don't follow it with reassurance. Let the silence sit.

## Part 4 — The reward (4 minutes)

Show the winning skill page.

17. What is this, and what would you do with it?
18. Would you rather have this, or the finished thing the winner actually made? Why?
19. There are two different things here: the AI usage from your own plan, and Daycare credits. What's the difference?
20. If you entered a challenge, you can use a skill during that challenge, but using it for your own work later costs credits. What do you make of that?

Questions 19 and 20 test comprehension of two decisions already made. If participants can't restate the two-currency distinction, or find the challenge-only rule confusing or unfair, that's a design finding rather than a copy problem.

## Part 5 — Access and memory (4 minutes)

Show the memory approval screen.

21. What is this asking you?
22. Which of these would you approve, and which would you not? Why?
23. Where's your line on this?

Then disclose the execution model plainly, without cushioning it:

> To do this, your agent runs on your own computer, using your own tools, in a folder you pick. Then it uploads what it made.

24. What's your reaction to that?
25. What would you need to know before allowing it?
26. Is there anything that would make this a no for you no matter what?

**Record the unprompted reaction to question 24 as closely to verbatim as possible, and note whether the concern is about the folder, the tools, the upload, or other people seeing the result.** Those are four different problems with four different fixes, and it's easy to treat them as one.

## Part 6 — Wrap (3 minutes)

27. If this existed today and worked, would you try it once? What would you expect to happen the first time?
28. Would you come back a second time? What would have to have happened?
29. What's the one thing you'd change?
30. Is there anything you expected me to ask that I didn't?

Close:

> That's everything. Thank you. Is it okay if I follow up if I have a question later? And if I want to quote something you said, I'll check with you first.

## Note sheet — one per participant

| Field | |
|---|---|
| Participant | Initials or ID only |
| Date, time, location | |
| How recruited | |
| Recording | Yes / no, with consent on tape |
| Stimulus used | Deployed homepage or local build |
| Pays for AI | Which tool and plan |
| Has hit a usage limit | Yes / no, what happened |
| Time to correct answer on Q5 | Seconds, or did not get there |
| Their words for the product | Exact phrasing |
| Understood the rubric | Yes / partly / no |
| Would enter, spending own allowance | Yes / conditional / no, and the condition |
| Skill or finished artifact | Which, and why |
| Restated the two currencies correctly | Yes / partly / no |
| Reaction to running on their machine | Verbatim, plus which of the four concerns |
| Memory items approved and declined | |
| Would try once | Yes / conditional / no |
| Would return | Yes / conditional / no, and the condition |
| Points where they got stuck | With severity, below |
| Direct quotes | Mark exact versus paraphrase. Never convert a recalled note into quotation marks |
| Contrary evidence | Anything that undercuts the premise |

## Severity

Rate each problem observed, so changes get ranked by evidence instead of preference.

- **Blocker** — the participant couldn't proceed, or said no outright and didn't move.
- **Major** — they completed the step but misunderstood something that affects their decision, such as cost, what runs where, or how they win.
- **Minor** — friction, wrong wording, or a question the page should have answered.
- **Cosmetic** — noticed but didn't affect understanding or the decision.

Count how many of the participants hit each problem. A problem three of five people hit is a finding. A problem one person hit is a note.

## How to read the results honestly

- Separate what people **did** from what they **said they would do**. Only the first is behavior.
- An answer to question 16 of "yes, that sounds cool" with no stated condition is a soft no. Record the condition, or record that there wasn't one.
- If nobody in Part 1 reports having hit a usage limit, the allowance framing is a hypothesis the sessions didn't support, and the write-up should say so.
- Five sessions give counts, not rates. Report raw numbers, never percentages.
