# Custom Instructions — Seattle job discovery

## Discovery coverage
Use portals.yml as the active list. Entries marked scan_method: websearch and all search_queries
require the agent scan workflow; node scan.mjs alone does not execute them.
Run available structured providers first, then complete the agent handoff using official employer
careers pages and official ATS listings. Prefer those sources over LinkedIn and aggregators.
If a provider fails, report the failure and use agent discovery; do not report zero vacancies as
a successful scan. Do not invent a provider or ATS tenant.
The configured ATS routes were identified from public careers sources on 2026-11-19;
configuration validation does not certify a successful live feed scan.
P1/P2 labels in notes are agent prioritization guidance, not scanner-enforced ranking.

## Eligibility review after discovery
For every shortlisted role, report WA eligibility as confirmed, needs verification, or ineligible,
with the posting URL and supporting wording. Remote alone is insufficient.
Check US and state restrictions, required office visits, travel, shift schedules and people-management duties.
The location filter is an initial candidate screen: missing locations and remote titles can pass.
Review unknown locations and generic US/Washington/multi-location results from agent discovery;
do not equate passing the scanner with eligibility.
For government roles, check public versus internal-only eligibility and closing dates.
For broad titles such as Program Analyst or Business Systems Analyst, confirm actual data/BI duties.
Deduplicate shared UW/UW Medicine and city department listings by canonical posting URL/requisition.
Report date posted separately from first seen; missing posting dates are unknown, not today's date.
Do not apply a 24-hour posting cutoff to undated roles or discard older still-open roles by default.

## Output
Use English for job reports. Include employer, title, source URL, location, work arrangement,
WA eligibility/evidence, posting date, first-seen date, closing date when available, compensation,
IC/management status and fit notes.
Summarize sources successfully checked, failed, and pending agent handoff separately.
This configuration change does not create a scheduler or alter any existing ChatGPT automation.
