> **Portability note:** This archived source-kit variant was written around a capable ChatGPT-style agent and Metricool. It is optional reference material, not the universal starter. Replace scheduler/image-tool steps with the services you actually use and verify their current official documentation, account access, plan limits, and costs. This document is guidance, not permission to connect, spend, schedule, or publish. For a tool-flexible workflow, start with the package-level `advanced-workflow.md`.

# Recovery, resuming, and real automation

Use these instructions alongside the master prompt. They preserve successful work and make blocked steps concrete.

## State model

| State | Meaning |
|---|---|
| DRAFT | Planned copy/design; not ready for use |
| GENERATED | Image tool returned an output; not approved |
| QA_PASSED | Required review completed; owner approval may still be pending |
| APPROVED_READY | Exact passing revision approved for this run |
| SUBMITTED_UNVERIFIED | Action attempted; native outcome not yet confirmed |
| SCHEDULED_VERIFIED | Correct account has saved schedule with confirmed time |
| PUBLISHED_VERIFIED | Actual public/owner publication status confirmed |
| BLOCKED | A specific dependency prevents progress |
| FAILED | Confirmed failure; preserve evidence and reconcile before retry |
| SUPERSEDED | Replaced creative, never select as final |
| CANCELED_VERIFIED | Native cancellation/removal confirmed |

Never advance status based only on intention or a local file update.

## Failure-to-action map

| Situation | Correct next step | Avoid |
|---|---|---|
| Missing logo/reference | Ask for the actual accessible asset; continue copy/planning | Inventing a new logo |
| Wrong client/account signed in | Stop writes; select/verify the correct authorized session | Using the convenient account |
| Same-name social profile | Seek ownership/admin evidence | Treating the name match as proof |
| OAuth return still loading | Inspect saved connection/account selector | Saying “connected” |
| Broad new permissions | Explain actual scope; follow action-time requirements | Treating scopes as ad-spending authority |
| Login/MFA needed | Preserve tab; request the precise secure human step | Asking for passwords/codes in chat |
| Binding terms or security challenge | Follow current required confirmation/handoff | Bypassing security or automatic consent |
| Free quota exceeded | Use approved fallback or prepare drafts | Buying a plan or claiming bulk import bypasses quota |
| Unsupported format | Propose an approved adaptation/route | Uploading a still image as a video |
| Trial ends before posts | Resolve supported route before schedule claims | Ignoring expiry |
| Extra wall/screen words | Narrow image edit and visual recheck | Accepting because the headline is correct |
| Logo or footer fails | Repair/hold exact asset and record defect | Claiming a perfect mark or hiding conditions |
| Repeated face | Change that primary person with invariants | Recoloring the same person |
| Upload button disabled | Inspect actual error/preview and supported route | Repeated blind clicks |
| File permission required | Explain exact step and apply active tool rules | Weakening security silently |
| Submit times out | Reconcile queue/history/ledger first | Duplicate resubmission |
| Local time reset in control | Verify saved native datetime | Trusting typed text |
| Offer expires during month | Replace future offer concept with approved evergreen or seek a new offer | Extending deadline automatically |
| Missed scheduled day | Report and agree next future slot | Dumping old posts in a catch-up batch |
| Agent/browser conflict | Stop simultaneous mutations; assign one operator | Fighting another worker’s UI actions |

## Resume prompt

~~~text
Resume this run from the attached account matrix, asset manifest, calendar,
QA record, and publication ledger. Read my latest instructions first.
Do not regenerate approved files, reconnect verified accounts needlessly,
or resubmit successful destinations. Verify current account identity,
queue/history, plan, offer validity, and the status of uncertain actions.
Complete only the unfinished authorized work. Preserve originals and
successful posts. Report exact counts and concrete blockers.
~~~

Attach the actual latest records and files, not just their filenames. A new chat has no automatic access to the old device/session.

## Add a platform without altering approved creative

~~~text
Prepare these existing approved assets for [EXACT ACCOUNT/URL].
Do not change the image, caption, or other schedules yet.
Inspect identity/admin access, supported format/link behavior,
scheduler tier/quota, and duplicate history. Give the proposed route,
dates, necessary adaptations, and blockers. I will choose the next action.
~~~

If the user later authorizes unchanged duplication, preserve exact image/caption hashes where supported, create new delivery IDs, and verify only the newly selected destination. Do not reinterpret permission as permission to rewrite or expand the batch.

## Recurring production specification

Use a supported automation tool only when the user requests actual recurring work. Fill every field:

- Brand and exact account allowlist.
- Source-of-truth/identity/asset locations.
- Job purpose: monitor / prepare drafts / generate / schedule / publish.
- Cadence, local time, named zone, next run, end date.
- Allowed content pillars and prohibited claims.
- Active offer expiry handling.
- Approval mode and required human steps.
- Generation/retry/subscription/ad cost caps.
- Monthly quota and existing queue reconciliation.
- Deduplication key and publication ledger path.
- Permitted native fallbacks.
- Stop conditions and error reporting.
- Notification preference.
- Explicit limits on account, access, spending, and campaign changes.

Default recurring production should not inherit an old ad budget or evergreen approval for a dated promotion. Verify fresh facts/queue at each run.

## Portable recurring-job prompt

~~~text
On each authorized run, read the latest brief, approvals, brand truth,
account allowlist, budget, asset records, and per-destination ledger.
Verify current account/plan/connection, existing queue, offer validity,
and the intended future period. Reuse approved assets where suitable.
Prepare or execute only the action allowed by the recorded review mode.
Do not create paid ads, upgrade subscriptions, change permissions,
edit unrelated posts, or expand destinations without current authority.
Reconcile uncertain submits before retries. Record exact outcomes,
costs, IDs, and evidence. Stop at the end date or a required dependency.
Follow the recorded notification rule; do not report unchanged
non-actionable states when quiet monitoring is requested.
~~~

A job prompt is a specification. The agent must save it in the actual available automation system and verify the returned job ID/status/next run. Otherwise label it “prepared, not installed.”

## Acceptance test for an installed workflow

- Correct job, brand, action scope, account allowlist.
- Correct schedule/time zone and finite end date.
- Current approval/budget/fact/offer sources.
- Deduplication and queue checks.
- Clear failure/notification behavior.
- Actual saved job ID and next run visible.
- A completed run produces verifiable records and native outcomes.

Do not run a live public “test post” or paid job without authorization. A read-only/draft dry run can check preparation while publication remains untested.
