# Firmware readiness review when silicon samples move

Published by Tymeline. Use this worksheet when a revised sample forecast could affect firmware bring-up, qualification or a customer release. The example is synthetic. Replace every revision, test reference and date with approved internal evidence before using it for a real commitment.

## Example review

Revision A1 samples were expected in week 10 and are now forecast for week 11. Firmware build F17 is ready for emulator regression against the current register map. The bench work still depends on A1, board revision B2 and lab capacity. The program team has proposed a change to the software development kit (SDK) preview date. That date remains a proposal until reviewed and approved.

| Work | Evidence to inspect | Decision to record |
| --- | --- | --- |
| Emulator regression | Firmware build, emulator image, register map revision, test scope | Record what can run now and which results will require confirmation on physical silicon. |
| Bench bring-up | Sample revision and confirmed arrival, board revision, lab booking and test plan | Record the earliest supported start and the dependencies still open. |
| Qualification | Applicable sample lot and configuration, procedure, required evidence and lab capacity | Determine whether the sample change affects qualification evidence or the qualification date. |
| Customer SDK preview | Dependency on bench results, committed release scope and approver | Record the proposed date separately from the current commitment and retain the approval reference. |

## Copyable review record

- Current committed milestone and owner
- Old sample forecast, new forecast and evidence reference
- Tested and expected silicon, board and firmware revisions
- Tests that can proceed and the scope of their evidence
- Physical tests still blocked and the owner of each dependency
- Proposed downstream dates and open assumptions
- Authorized reviewer, decision, decision time and evidence reference

Once the responsible engineer confirms which evidence applies, the authorized program owner can decide whether to change the commitment. Keep the underlying evidence and decisions in the approved program environment. [Tymeline firmware readiness guide](https://tymeline.ai/resources/firmware-readiness-silicon).
