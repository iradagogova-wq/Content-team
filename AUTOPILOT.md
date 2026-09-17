# Content Autopilot

This repository now supports a closed-loop Instagram content system.

## Architecture

**ChatGPT = strategist + copy + quality control**

Reads brand rules, prior ideas, research, recent results and current analytics. Chooses the next content hypothesis and creates the complete publication package.

**GitHub = long-term operating memory**

Stores brand rules, research, content calendar, experiments, results and machine-readable state. This prevents the system from forgetting what was already tested and why the next post was chosen.

**Metricool = publisher + primary analytics layer**

Once connected to ChatGPT and the target Instagram account, it is the preferred layer for scheduling/publishing content, recommended posting times and performance metrics.

**ChatPlace = optional Instagram automation + Virale intelligence**

The connected Instagram bot can be used for DMs, comment funnels and Virale intelligence. AI media generation is optional and should only be used when sufficient ChatPlace AI credits are available.

## Why this replaces the old manual release step

`PLAYBOOK.md` remains the manual workflow and is not overwritten. Autopilot is a separate mode for recurring publication.

Autopilot follows:

`analytics -> learning -> hypothesis -> content -> quality gate -> media -> publish -> 24h/72h metrics -> next hypothesis`

The system must never confuse correlation with proof. Performance observations are facts; explanations for why they worked are hypotheses until repeated tests support them.

## Files

- `autopilot/config.json` — account, tool priorities, cadence and quality gates.
- `autopilot/state.json` — current machine state, experiments, winners and pending work.
- `autopilot/daily-agent-prompt.md` — exact operating procedure for the recurring agent.
- `brand/*` — source of truth for voice, psychology and scenario quality.
- `research/*` — evidence and niche maps.
- `pipeline/*` — ideas, scripts and publication calendar.
- `results/*` — measurements and experiment conclusions.

## Current bootstrap status

- Instagram bot connected in ChatPlace: `@irada.gogovapro`.
- GitHub repository ready: `iradagogova-wq/Content-team`.
- Metricool connection: required before autonomous publishing can be considered live.
- ChatPlace AI credits at bootstrap: 0; Virale generation must not be treated as a required dependency.

## Definition of LIVE

The autopilot is live only when all of the following have been verified in a real run:
1. Metricool is connected to the correct Instagram brand.
2. The agent can read current performance metrics.
3. A media asset can be produced without a manual approval bottleneck.
4. A test publication is scheduled or published to the correct account.
5. The resulting post can be found again and measured.
6. The measurement is persisted to GitHub and changes the next content decision.

Do not claim the system is fully live before this end-to-end test succeeds.
