# Supplier IP delay review for semiconductor programs

Published by Tymeline. Use this manual review when an IP supplier revises a delivery forecast. Keep completed records and supplier communications in your approved program environment.

## Synthetic exercise

An IP delivery moves from March 2 to March 9. Integration was planned for March 4. Assume the existing integration build uses a prior IP revision. Ask the responsible engineers which tests can proceed on that revision and which results need to be repeated on the new drop. A revised supplier forecast is an input to the decision. The committed integration and tape-out dates change only through the applicable approval workflow.

| Review | Evidence | Decision |
| --- | --- | --- |
| Supplier forecast | Dated source message, affected revision, and delivery owner | Confirm what the supplier actually committed to and record any unknowns. |
| Integration and verification | Dependency map, revision used by each test, and coverage scope | Identify blocked work and tests that can proceed. Record any limits on reusing results. |
| Firmware and lab work | Relevant interface revision, emulator image, lab booking and sample dependency | Check which assumptions still apply and who will validate them. |
| Recovery options | Alternate drop, proposed work sequence, people and lab availability | Record the cost and schedule assumptions for each option. |
| Commitment review | Current baseline, proposed dates, evidence and designated approver | Record the approved change or rejection, the date and the evidence reference. |

Ask each owner to confirm the source and affected work before relying on a revised plan. The example uses synthetic dates and establishes no recovery time or performance result. [Tymeline's supplier-delay guide](https://tymeline.ai/resources/catch-supplier-delay-before-tape-out).

## Test the same evidence chain across vendors

Set up three records in a test workspace or import sample records. All identifiers and dates here are synthetic.

| Source | Sample record | Check |
| --- | --- | --- |
| Jira milestone | INT-017, integration planned March 4, assigned to the integration lead | The review shows the current milestone, its owner and the dependency on the new IP. |
| Perforce revision and verification record | Change 4812 contains the previous IP revision. VER-041 is a passing regression against that change. | The review shows which revision was tested. The verification owner decides which tests must be repeated after the new drop. |
| Supplier message | A dated update revises the delivery forecast from March 2 to March 9. | The review preserves the prior forecast, the revised forecast and the source message. |

Ask each vendor to show the affected work, assumptions, recovery proposal and approval record. Try a proposed change with a user who lacks approval authority. Confirm the proposed date and existing commitment are distinguishable. Then have the authorized approver record a decision, and check which actions and evidence appear in the decision history.
