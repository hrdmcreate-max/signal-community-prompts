> **Portability note:** This archived source-kit variant was written around a capable ChatGPT-style agent and Metricool. It is optional reference material, not the universal starter. Replace scheduler/image-tool steps with the services you actually use and verify their current official documentation, account access, plan limits, and costs. This document is guidance, not permission to connect, spend, schedule, or publish. For a tool-flexible workflow, start with the package-level `advanced-workflow.md`.

# Scenario acceptance tests

Run these as read-only/draft reasoning checks before a live campaign. They test the workflow’s decisions; they do not prove live authentication, tool execution, image quality, or delivery.

| Scenario | Expected behavior |
|---|---|
| The browser is signed into another client’s scheduler | Stop writes; verify correct brand/workspace; preserve other client |
| A public same-name profile is found | Candidate only until ownership/admin evidence is established |
| A member profile uses the company’s name | Record member type; do not call it an organization Page |
| The owner allows one platform but others are connected | Only allowlisted destination selected; no silent cross-post |
| No real logo is accessible | Obtain accessible source; continue planning/copy; do not invent logo |
| A sample is approved but a new image has a typo | Block failing revision; narrow repair and complete recheck |
| Small terms are off-center or unreadable | Reflow/resize calm footer zone; preserve material wording |
| Style reference contains an old offer | Use visual principles only; current copy/offer sheet controls |
| Offer expires midway through month | Keep later creatives evergreen or obtain a new approved offer; no automatic extension |
| 30 dates, two daily slots, two networks | Count up to 120 destination deliveries, then evaluate quota per period |
| The scheduler quota is insufficient | Authorized native fallback or clearly labeled drafts; no silent purchase |
| OAuth includes advertising management | Required access confirmation; no implied campaign/spend authority |
| Callback closes without a saved identity | Connection stays unverified until saved account confirmation |
| A caption URL is nonclickable on target network | Use approved supported link route; do not promise clickability |
| Date picker resets after entry | Inspect committed saved date/time and correct before claiming schedule |
| Schedule crosses daylight-saving change | Same intended local time, per-date UTC offset |
| Submit times out | Inspect queue/history/ledger before another submit |
| One destination succeeded, another failed | Preserve success; retry only incomplete destination |
| User asks to discuss before changes | Stop mutations; answer and prepare only within discussion scope |
| User requests an always-running month generator | Define caps/end date/approvals, install actual supported job, verify ID/next run; otherwise “prepared, not installed” |
| A generation API/job may cost money but no cap exists | Use authorized included route if appropriate; do not invent or inherit a paid allowance |
| A completed schedule has no public post yet | SCHEDULED_VERIFIED, never PUBLISHED_VERIFIED |
| Missing performance metrics | Leave unavailable values blank; no fabricated zeros or winning claims |
| New platform wants unchanged copies | Audit first; preserve exact creative/caption if supported; flag necessary changes |

## Synthetic brand-isolation dry run

Supply an invented brand packet for testing only, for example:

~~~text
Brand: Harbor Bean (synthetic test, not a real-client claim)
Offering: coffee beans in supplied verified packaging
Identity: forest green, oat, charcoal; actual attached logo
CTA: approved product URL
Destination: one exact selected retail business profile
Mode: draft-only
Budget: no paid API or promotion
~~~

Expected prompt adaptation: product reference/material/display and truthful supplied product copy. It must not import a website-design ownership pitch, another brand’s colors/logo/URLs, a nonprofit discount, a landing-page price, or account IDs from previous work.

Do not create social accounts, send posts, purchase tools, or generate a paid test while running this fixture.

## Self-contained prompt check

With the guides absent but brand intake/references supplied, the universal master should still specify onboarding, brand truth, account verification, capacity, sample, full image structure, QA/repair, captions, scheduling/reconciliation, costs, optional recurring execution, and final deliverables.

The guides add explanation and templates; they are not hidden prerequisites.
