# The Babysitters — Weekly update, November 6, 2026

**Claude Daycare** · Mitchell Rosenthal, Almog Ankori, Josh Hegstad, Mansi Rank

## What we built last week and why

The week went into product direction rather than features. We consolidated two parallel idea threads into a single working brief, inspected our own platform repo read-only against the new direction to find out what we actually have, settled five architecture decisions that had been blocking the build, and wrote a moderated usability script for the assumptions the new direction rests on.

We did that instead of shipping another activity because of the midterm feedback. People told us they were nervous about what our agent could reach and unwilling to spend their own paid allowance on a visit. Both are the same question asked twice, which is what an owner gets for sending their agent at all, and a sixth activity wouldn't have answered either one.

The direction we landed on: several challenges run at once, agents enter solo under a published brief, results are judged on the brief's goals plus real human preference, and the winning approach becomes a reusable skill other owners can unlock with credits. The reason to return is a skill that helps with the owner's own work.

The repo inspection was the most useful part. We have activity discovery, seats, configurable rules and a turn engine that validates legal moves. We have no submission, judging, scoring or reward machinery for artifacts, and no skill library at all. That tells us the event lifecycle is the build, not a feature layered onto a working platform.

## What we're building this week and why

One complete event lifecycle end to end for a single challenge: draft, open, submissions closed, human judging, finalized. Solo entry, rules frozen once a round is live, submission, completion checks, voting, and a result the entrant can read.

The lifecycle comes before more challenges because every category reuses it and because none of the rest of the plan can be tested until one round can actually finish.

Alongside it, rewriting the runner launch and the trust page to match the new execution model, and running the first usability sessions with strangers.

## Current user count

0 confirmed users. Four local signup forms pass database save and readback and GA Realtime lists all four routes, but production capture has not been verified and no real public signup has been stored and read back. We are counting a stored signup on the deployed site as the threshold and nothing weaker.

## Biggest blocker

Our execution decision contradicts our own trust story, and we haven't decided what replaces it.

The runner today launches the agent into a throwaway workspace with no file, shell, or browser access, and our trust page describes that isolation as the reason to trust us. It's also what we pointed at whenever someone raised security. We've now decided agents should work on the owner's real machine with their real tools, in a folder the challenge specifies. That's a much more useful product and a much larger surface to worry about, and the honest reading is that we increased the risk in response to feedback that we were already too risky.

We can't ship the new direction without rewriting both the launch and the page, and we can't write the page until we decide what promise we're making instead. That decision gets worse the longer we build around it, which is why it's ahead of the two other open items: that the skill library doesn't exist yet, and that challenge-only skill access is currently a rule rather than a mechanism.
