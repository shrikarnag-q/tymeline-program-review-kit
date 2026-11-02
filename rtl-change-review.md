# Post-freeze RTL change review worksheet

Use this Tymeline worksheet to prepare a proposed engineering change order (ECO) for the people who own verification, physical design and the program date. After register-transfer-level (RTL) freeze, capture changes against the controlled design baseline so reviewers can see which existing results still apply.

## Copy into your change record

| Field | What to record |
| --- | --- |
| Change and baseline | ECO reference, frozen RTL revision, proposed revision, affected block or interface and reason for the change |
| Options | Apply now, defer, or take a specific alternative. Record the consequence of each choice. |
| Evidence and applicability | Existing regression, coverage or physical-design reports, the revisions they cover, and the checks an engineer considers affected |
| Re-verification | Required checks, owners, completion criteria, and prerequisites for the chosen option |
| Milestone impact | Affected milestone, schedule impact range or unknown, basis for the estimate, and dependencies that could change it |
| Technical decision | Authorized change approver, disposition, conditions and decision record |
| Program decision | Accountable owner, any date or scope change, and the decision record |
| Closeout | Implemented revision, completed verification evidence and remaining exceptions |

Use your program’s approval rules. Keep authorization to implement, evidence of verification and any decision to move the program date as separate records. A schedule impact estimate can remain unknown while engineering collects evidence.

## Illustrative example

A proposed change alters reset behavior at an interface after freeze. The existing integration regression was run on frozen revision `RTL-A`. The proposed revision `RTL-B` has yet to be tested.

The verification lead reviews which reset and integration checks must be repeated. The physical-design lead checks whether timing or implementation reports need to be refreshed for the affected logic. The program owner records the potential effect on the sign-off milestone once those leads confirm scope and capacity. Until then, schedule impact is unknown and technical approval is pending. The review record links any later approval to the exact revision and evidence considered.

Keep actual revisions, artifacts and approval records inside your authorized environment. The example uses synthetic revisions and describes a manual review.

## Related guides from Tymeline

- [RTL freeze and engineering change control](https://tymeline.ai/resources/rtl-freeze)
- [ECO impact across a chip program](https://tymeline.ai/resources/eco-impact-analysis)
- [AI agents and human approval in semiconductor program management](https://tymeline.ai/resources/ai-agents-semiconductor-program-management)
