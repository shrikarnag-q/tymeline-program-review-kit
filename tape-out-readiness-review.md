# Evidence-based tape-out readiness review worksheet

Published by Tymeline for semiconductor engineering teams. Use this manual worksheet to connect release criteria to evidence for the exact design revision proposed for tape-out.

## Blank review record

- Program and release candidate
- Target submission and review time
- Applicable gate criteria and foundry process
- Engineering owners and authorized decision maker
- Final decision, scope and approval reference

| Release criterion | Candidate revision | Evidence artifact and observation time | Evidence revision | Engineering owner | Status | Next action or approval reference |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |

Use a separate row for each criterion or exception. Record the reason an earlier result applies only after the responsible engineer evaluates it. Keep any proposed waiver open until its authorized approver records the decision and scope.

## Worked example

All revisions, references and observations below are synthetic. The example release candidate is R17.

| Release criterion | Candidate revision | Evidence artifact and observation time | Evidence revision | Engineering owner | Status | Next action or approval reference |
| --- | --- | --- | --- | --- | --- | --- |
| Static timing covers the approved sign-off scenarios | R17 | TIM-016, March 4 at 14:00 UTC | R16 | Timing lead | Pending | Obtain R17 evidence or record an approved applicability determination |
| Physical rule-check exception has a recorded disposition | R17 | PHY-017, March 5 at 10:00 UTC | R17 | Physical verification lead | Waiver proposed | Record the waiver's scope and approval, or resolve the exception |
| Required functional regression suites are reviewed | R17 | VER-017, March 5 at 11:00 UTC | R17 | Verification lead | Evidence available | Confirm coverage of the required suite and record the review |
| Tape-out gate is authorized | R17 | Gate packet draft, March 5 at 12:00 UTC | R17 | Release approver | Decision pending | Review the open rows and record the authorized gate decision |

## Review the packet

1. Check that each evidence artifact identifies the revision, relevant run configuration and observed result.
2. Separate missing evidence, earlier-revision results and proposed waivers. Assign each open item an owner and next action.
3. Record the approval or deferral, the revision and scope it covers, and the decision reference. Keep controlled project records in the approved engineering environment.

[Tymeline’s tape-out readiness guide](https://tymeline.ai/resources/tape-out-readiness-review) explains the role of the decision packet. [Tymeline chip programs](https://tymeline.ai/semi-conductor) describes the program coordination workflow.
