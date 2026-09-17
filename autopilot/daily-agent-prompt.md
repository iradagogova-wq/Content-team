# DAILY CONTENT AUTOPILOT

Run this as a closed-loop publishing agent for the Instagram account configured in `autopilot/config.json`.

## Goal
Create and publish one high-quality Instagram content unit per day, learn from its performance, and use that evidence to improve the next publication. Do not optimize for posting volume. Optimize for saves, shares, qualified attention, profile actions, leads, and sales intent.

## Read before every run
1. `autopilot/config.json`
2. `autopilot/state.json`
3. `brand/voice.md`
4. `brand/scenario-standard.md`
5. `brand/psychology.md`
6. `brand/swipe-file.md`
7. `pipeline/ideas.md`
8. `pipeline/calendar.md`
9. the newest relevant files in `research/` and `results/`

Never silently change a locked brand rule. If repository instructions conflict, prefer the newest explicit rule that is clearly marked as approved/final.

## Daily cycle

### 1. Measure first
Use Metricool as the primary analytics source once connected. Pull recent post/reel/carousel performance and recommended posting time. Record 24h and 72h snapshots when those windows become available.

Compare each post against the rolling median of the last 10 posts of the same format, not against raw follower count alone. Prioritize these signals when available:
- shares / reach
- saves / reach
- follows or profile actions / reach
- comments / reach
- watch time, retention or completion for video

If a metric is unavailable, do not invent it. Use the strongest available substitutes and record the limitation.

### 2. Extract one actionable learning
Write one short evidence-based statement in this form:
`Observed pattern -> likely reason -> what to test next.`

Separate fact from hypothesis. Do not copy a winning post literally; preserve the mechanism and change the angle, proof, example, or framing.

### 3. Choose today's content
Use the mix from `autopilot/config.json`:
- 70% proven patterns
- 20% adjacent tests
- 10% exploration

Avoid repeating the same hook, topic, visual opening, or CTA from the recent calendar unless intentionally running a controlled iteration.

Choose the format using evidence. Do not force carousels if reels are materially stronger, and vice versa.

### 4. Build the publication
Create the complete content package:
- objective
- audience/job-to-be-done
- hook
- full script or slide copy
- caption
- CTA
- visual brief
- publication time
- hypothesis being tested

Run the brand and psychology checks before creating media.

### 5. Create media
Preferred order:
1. ChatGPT image generation for original static/carousel assets when available.
2. ChatPlace Virale only when its AI balance is sufficient and its output is suitable.
3. Existing approved brand assets/templates where they can be used without blocking on manual approval.

Never publish a low-quality placeholder merely to satisfy the daily cadence. If media generation fails, keep the package queued and report the exact blocker.

### 6. Publish
Use Metricool once connected. Schedule for Metricool's recommended audience time when reliable; otherwise use the best recent audience window supported by data.

Before publishing, verify:
- correct Instagram account
- all carousel pages in correct order
- readable crop and aspect ratio
- no accidental duplicate post
- caption and CTA are final
- no unsupported health, financial, legal, or performance claims

### 7. Persist state
After publishing, update `autopilot/state.json` with:
- run timestamp
- media/post id or URL when available
- topic and format
- hook
- hypothesis
- scheduled/published time
- metrics snapshot placeholders for 24h and 72h

Append the publication to `pipeline/calendar.md` and the test idea/result to the appropriate file under `results/`.

### 8. Weekly recalibration
On the first run each Monday, also review the last 30 days:
- strongest repeated mechanisms
- declining mechanisms
- format shifts
- topic saturation
- conversion-oriented content vs reach-only content

Update the next 7-day hypothesis set. Do not throw away a working system because of one weak post.

## Failure behavior
- If Metricool is not connected: create the finished package and store it, but do not claim it was published.
- If ChatPlace AI credits are zero: skip paid Virale generation; do not burn time retrying.
- If analytics are incomplete: proceed using verified available metrics and mark uncertainty.
- If a tool fails: attempt one sensible fallback, then record the blocker. Do not loop repeatedly.

## Output after each run
Return only a concise operational report:
`Published/Scheduled | format | topic | hook | hypothesis | why this was chosen | next measurement window`.
