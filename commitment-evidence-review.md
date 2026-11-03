# Semiconductor program commitment evidence review

A manual evaluation exercise from Tymeline for engineering program managers. Use it to test whether a coordination platform can trace a delivery commitment to versioned engineering evidence and show exactly what still needs a human decision.

## Set up one commitment

Use synthetic records in a sandbox. Keep the original commitment and each revision of its supporting evidence accessible to the authorized reviewers.

| Record | Example | What to preserve |
| --- | --- | --- |
| External commitment | Sample delivery on November 30 | Original date, decision owner and approved record |
| Program dependency | Jira work item CHIP-42 blocks sample release | Link type, owner and source URL |
| Candidate revision | Submitted P4 changelist 4102 | Immutable revision reference and access scope |
| Verification result | Run EX-109 passes against changelist 4098 | Tested revision, configuration, outcome and observed time |
| Decision | Release approval pending | Proposed action, assigned approver and eventual signed record |

## Run the same checks with each vendor

1. **Check applicability.** Ask whether the candidate is ready. Expect the answer to distinguish the passing run on 4098 from the unverified candidate at 4102. The responsible engineer determines whether the earlier result applies or a rerun is needed.
2. **Supply fresh evidence.** Add a passing run for 4102. Expect the answer to update the evidence assessment and preserve the November 30 commitment and its approval state.
3. **Check restricted access.** Repeat as a user who cannot read the changelist or run. Inspect the answer, generated digest and activity log for restricted identifiers, excerpts or results. Record what the user can independently verify.
4. **Separate proposals from approvals.** Ask for a revised customer date. Expect a proposal with supporting sources and the assigned approver. Check the original record and downstream systems for unintended writes or notifications.

For each check record the observed result, the source link or audit event, and a pass, fail or untested outcome. Keep connector availability, permissions and audit retention explicit. Use the same evidence, roles and evaluation window across platforms.

## Sources and related workflows

[Jira timeline dependencies](https://support.atlassian.com/jira-software-cloud/docs/manage-dependencies-between-epics-on-the-timeline/) describes how linked work items express sequencing. [Perforce changelist documentation](https://help.perforce.com/helix-core/server-apps/cmdref/current/Content/CmdRef/p4_describe.html) describes submitted changelists and restricted visibility.

Use the [supplier IP delay exercise](supplier-ip-delay-review.md) for an external forecast change or the [tape-out readiness exercise](tape-out-readiness-review.md) to review sign-off evidence. [Tymeline's semiconductor program management guide](https://tymeline.ai/resources/semiconductor-program-management-software) describes its approach to coordinating engineering programs. This worksheet is an illustrative evaluation protocol.
