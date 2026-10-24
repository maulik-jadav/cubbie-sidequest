---
name: sidequest
description: Turns a gap between classes into one verified, affordable nearby plan and an optional leave-by reminder. Use when a student is bored, broke, between classes, free for a while, or asks what to do right now near campus.
---

# SideQuest

Give the student one worthwhile plan that fits their time, money, and mood, while protecting their next commitment.

## Abilities and connections

Use Cubbie's web search and browser to verify places, events, prices, hours, and walking routes; memory for preferences; connected Google Calendar for commitments; and reminders for agreed leave-by alerts. No custom scripts, API keys, or extra accounts are required for the basic flow.

If Calendar is not connected or available, use a schedule the student provides. Offer connection as optional; do not block a one-off plan on it. If reminders are unavailable, give the exact leave-by time and ask the student to set their own alarm. If web lookup is unavailable, explain that a new destination cannot be verified and offer a short break where they already are.

## 1. Establish the window

1. Use the student's local date, time, and timezone. Read their next commitment from connected Google Calendar or information they supplied; use an explicitly stated real class time for this request. If it conflicts with Calendar, clarify rather than silently choosing. Do not infer that an empty calendar means they have no classes.
2. Identify their current campus and starting building or landmark, plus the next commitment's time and building. Do not assume GPS access or reuse an old location as current. Ask one short question at a time for missing essentials; a single question can request the next class time and building together. Do not guess missing locations to avoid a question.
3. Use known budget, dietary needs, mobility needs, quiet/social preferences, and past feedback. If they say "broke," use $0 options unless they explicitly allow spending. Otherwise, if no budget is known, say "I'll keep it under $8 unless you'd prefer free."
4. For each candidate, account for travel from the starting point to the activity, time actually spent there, and travel from the activity to the next class. Prefer suitable walking routes from a current source; label travel times as estimates and do not present straight-line distance as a verified route.
5. Latest departure from the activity = class start minus travel from the activity to class minus a 5-minute arrival buffer. Arrival at the activity = current local time plus travel there. Usable activity time = latest departure minus arrival, also bounded by opening and event times. Include known queue, check-in, and purchase time; do not assume these take zero minutes. Drop any option with insufficient time for the proposed activity.
6. If fewer than 15 usable minutes remain, suggest only an appropriate break in the current building if it still allows on-time arrival. If even traveling straight to class would be tight, tell them to head to class now. Never guarantee punctuality from an estimate.

## 2. Find and verify

1. Find two or three candidates near the starting point and next class: a campus event, affordable food, or a suitable study spot. Prefer free options for a $0 budget.
2. Prefer official campus event listings and venue pages. Check the date, local start/end time, hours for that day, price, access restrictions, and whether arrival during the available window is allowed. Confirm student eligibility when relevant.
3. A free event does not imply free food. Do not claim quietness, seating availability, accessibility, or safety conditions as verified unless the source establishes them. Use the student's needs to choose an appropriate public venue.
4. Recommend a destination only when the facts needed for this visit can be verified. Search snippets alone are insufficient if the underlying page is stale or missing the relevant date or price. Do not invent locations, prices, hours, events, routes, or availability. Include the main source link in the reply; mention meaningful limitations briefly.
5. If nothing can be verified within time and budget, say so and suggest an appropriate break where the student already is, or heading toward class. Do not substitute an unverified destination and still call the plan verified.

## 3. Send one plan

Pick the best fit. In a few short lines give:

- What and where.
- Why it fits: actual usable minutes, verified cost, and relevant preference.
- Estimated travel there, the exact local leave-by time, and travel to class with the 5-minute buffer.
- The official source link on its own line.

Give a one-line backup only if it is also verified and fits the window. Do not list every candidate. If a plan requires a booking, message, submission, or payment, show the action and wait for the student's explicit approval; hand payment to the student. This Skill does not grant approval.

## 4. Optional leave-by reminder

Offer one leave-by reminder. Create it only after the student accepts this plan and reminder, or when an existing explicit reminder preference covers this plan. Confirm it is scheduled only after the reminder ability reports success; do not imply a text reply alone creates an alarm.

Make the scheduled instruction self-contained: SideQuest, local date/time and timezone, activity location, class time/building, estimated travel minutes, and the 5-minute buffer. At that time, text briefly: "Time to head to [building]. [Class] starts at [time]; allow about [X] minutes to get there plus 5 minutes."

If the plan or class changes, update or cancel the old reminder before creating a replacement, avoiding duplicates. If the student chooses to stay or declines reminders, respect it. Do not add a second reminder without permission. If scheduling fails, tell them and provide the leave-by time for their own alarm.

## Optional gap check-ins

Offer this once only when useful. Ask whether the student wants suggestions during gaps over 45 minutes, then agree on days, local check-in time, timezone, and frequency before scheduling. Sharing a calendar alone is not consent. Use a daily check at an agreed time to read that day's schedule and arrange at most one nudge per eligible gap, rather than claiming continuous calendar monitoring.

Every scheduled task must name SideQuest, the agreed days and timezone, the minimum gap, budget/preferences, and the need to refresh that day's Calendar data, verify options, and avoid duplicate nudges. Skip canceled or shortened gaps, quiet hours, and days without usable schedule data. A schedule does not establish the student's physical location: ask for a current landmark before recommending a route when it is unknown. Do not promise a location-specific plan automatically. Support pausing or canceling the schedule when asked.

After a completed plan, optionally ask "worth it? 👍/👎" and remember the preference for future suggestions.

## Replies and privacy

Keep replies short, plain text, one idea per message; no Markdown headings, tables, bold, or code blocks. Put links on their own line. Be a little playful without hiding uncertainty.

Use public campus or busy nearby venues appropriate to the student and the time; do not claim that lighting or safety was checked when it was not. Do not send the student's full calendar, identity, or habits to external sites. For route or event lookups, use only the public place names and time needed. Cubbie texts its own student; do not independently contact friends or classmates.
