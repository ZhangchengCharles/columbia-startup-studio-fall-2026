# HW8 — Usability testing

## Sessions

**Three completed sessions.** This meets the class's requested count of 3–5 sessions. Further sessions can retest the proposed improvements. Tasks within a session are not counted as separate participants; a session can include tasks requiring assistance or remaining incomplete.

| Session | Evidence | Outcomes |
| --- | --- | --- |
| P01 | [Participant's written report](sessions/participant-01-report.txt) | Found Penn Station LIRR after relaxing filters; reported completing signup and saving; located Rate and Comment without submitting feedback. |
| P02 | [Team-reported session report](sessions/participant-02-report.txt) | Found a Starbucks restroom and passcode; understood missing information; confirmed saving and reopening; submitted a restroom that appeared after moderator approval, with hours missing. |
| P03 | [Team-reported session report](sessions/participant-03-report.txt) | Navigated the map and located themselves; opened a Central Park listing; found expanded issue text unclear; saved and reopened successfully; needed guidance to submit an entry-permission report and could not see the update where expected. |

The supplied accounts do not specify participant identities, recruitment methods, session dates, durations, app builds or devices. No timing or recording evidence was supplied. P01, P02 and P03 are anonymous session identifiers. P02 and P03 summarize the team's accounts rather than verbatim participant transcripts.

| Task | Reported result | Remaining check |
| --- | --- | --- |
| Find a suitable restroom | P01 recovered from an empty Clean + Public result. P02 found a Starbucks listing and passcode. P03 navigated, located themselves and opened the Pilgrim Hill and Conservatory Water listing, but found its expanded issue text unclear. | Retest filter recovery and readability of issue reports. Finding a code or seeing an issue count does not verify conditions at the venue. |
| Save a restroom for later | P01 reported signup and saving and found Saved places. P02 and P03 successfully saved and reopened a restroom; P02 reported no sign-in interruption. | Initial account states for P02 and P03 were not supplied; test fresh sign-in and return-to-map explicitly. |
| Share useful information | P01 found Rate and Comment without submitting feedback. P02's new restroom appeared after approval but lacked hours. P03 selected Public access for Entry permission, needed guidance to click Share, and did not see the update in Amenities afterward. | P03's submission and publication status remain unconfirmed. Check the full contribution-to-display workflow. Public-note and rating submission remain untested. |

## What we observed

1. **Basic navigation worked across the sessions.** P01 found the map, filters, bookmark and account sections without assistance. P02 described the controls and information as intuitive. P03 navigated the map, located themselves and opened a Central Park listing.
2. **Filter recovery caused difficulty in P01.** Clean + Public produced “No restroom was found.” P01 removed Clean but could not tell whether locations had poor cleanliness or lacked cleanliness information. P02 did not report encountering this empty result.
3. **Participants interpreted missing information differently.** Missing amenities and ratings reduced P01's confidence. P02 understood these as gaps in an early-stage app's data. Missing information does not establish that a restroom has no amenities or is unclean.
4. **Saving and reopening worked for P02 and P03.** P01 identified the account step as potential friction. P02 reported no sign-in interruption and confirmed saving and reopening; P03 also saved and reopened successfully. Their starting account states were not supplied.
5. **New-restroom publication worked, but the hours workflow was incomplete.** P02's submission appeared on the map after team approval. Its hours were missing, so P02 returned to look for a way to add them and suggested that the search returning an address could also return hours. The account does not establish whether hours were entered originally or where they became missing.

6. **Reported issues were discoverable but unclear for P03.** The Central Park listing showed three issues in Condition. P03 expanded Condition and the reported issues but found the text disorganized and difficult to understand. This is a presentation finding, not an independent inspection of three restroom defects.
7. **Contribution actions and outcomes were unclear for P03.** Through Amenities → Report a problem, P03 selected Public access under Entry permission, looked for Save and did not understand Share. The facilitator explained the action before P03 clicked it. The update did not appear in Amenities, where P03 expected it. The account does not establish whether it was saved, pending review, shown elsewhere or failed.

Basic navigation and saving worked, but contribution completeness and visible outcomes caused difficulties in P02 and P03. Each specific issue still comes from a small number of sessions; we have not established its frequency across users.

## What we will change

These are planned changes, not fixes confirmed by this session.

| Priority | Planned change | What we will check next |
| --- | --- | --- |
| 1 | Organize expanded issue reports into separate labeled items with short descriptions and available observation dates. | Can a participant explain the reported issues after expanding Condition? |
| 1 | Give the contribution action a clear label matching its behavior, such as Submit report or Save changes, and show success, review or error feedback. | Can a participant submit an entry-permission update without guidance and explain what happened? |
| 1 | Make the submitted field and its destination clear. Check persistence, review status and display of entry-permission updates; keep entry permission distinct from amenities. | Can a participant find their submitted information or its review status afterward? |
| 1 | Explain that no locations match the selected filters and offer a way to remove an individual filter. | Can a participant recover without reopening filters and guessing what went wrong? |
| 1 | Distinguish no cleanliness ratings from low ratings, and unreported amenities from confirmed absence. | Can a participant explain what is known and unknown before choosing a restroom? |
| 1 | Provide a clear optional hours field in new-restroom submissions and show those hours during moderator review. Investigate whether place lookup can suggest hours for the contributor to review. | Can a participant add hours, have them reviewed and see them on the approved map listing? Venue opening hours must remain distinguishable from restroom hours. |
| 2 | Retain the save-and-reopen flow that worked for P02 and P03 and check fresh sign-in continuation. | Can a new account save, reopen the place and return to the map without searching again? |
| 2 | Check that Add a public note clearly explains optional observations, public visibility and the result of submission. | Can a participant submit a note and find it afterward? |

## Why

The three sessions suggest people can navigate, find listings and save places, while understanding incomplete information and contributing updates need more work. P02's approved listing lacked hours. P03 needed help to submit and then could not see the information where expected. We will prioritize readable issue reports and a contribution workflow with clear actions, review status and visible results, alongside the hours and filter improvements. Follow-up sessions should retest those changes and cover fresh sign-in and public feedback submission.

Course requirement: [Class 8 slides, “What to submit by Friday, November 6”](../../../classes/20261030_c8w8_fri_post-mvp-and-prioritization/class-8-slides.html).
