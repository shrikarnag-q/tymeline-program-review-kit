# Governed AI coordination for hardware programs

A manual evaluation exercise published by Tymeline. Run it in a sandbox with synthetic records to compare how platforms handle a proposed board change across design, firmware, qualification and program management.

## Prepare the scenario

A power-management component becomes unavailable. An engineer proposes a substitution for board revision B. Revision A is the current released board. A firmware build and a thermal test report both refer to revision A. A customer qualification slot is reserved for revision B.

| Record | Evidence to load | Decision owner |
| --- | --- | --- |
| Design change | Proposed component substitution, schematic revision and affected bill of materials | Design change authority |
| Firmware compatibility | Build ID, supported board revision and verification result | Firmware lead |
| Qualification | Tested board revision, test report and lab slot | Qualification lead |
| Customer commitment | Approved date, assumptions and decision record | Program commitment owner |

## Run four checks

1. **Find the affected work.** Ask the platform to show the revised design artifact, connected firmware work, qualification evidence and customer milestone. Trace each conclusion to its source and record which relationships require manual mapping.
2. **Keep evidence tied to its revision.** Mark the revision A thermal test as passed. Ask what evidence supports revision B. The review should preserve the original pass and identify the need for an applicability decision by the qualification owner.
3. **Test authority and access.** Run the same review as a program coordinator who can see the milestone but lacks access to the schematic and cannot approve a design change. Check the displayed answer, export and activity log for unauthorized details or writes.
4. **Separate the decisions.** Have the authorized design lead approve the component substitution in the sandbox. Confirm the design decision is recorded with its evidence. Check that any proposal to move the customer milestone remains pending with its own approver.

Copy the [evaluation scorecard CSV](governed-hardware-coordination-scorecard.csv) for each platform. For each check record the observed behavior, evidence link or audit event, responsible role and pass, fail or untested result. Confirm available integrations, permissions and retention in the deployment you intend to use.

The [hardware program management buyer guide](https://tymeline.ai/resources/hardware-program-management-software) explains how to compare tools for design control, verification and delivery coordination. Use the [commitment evidence review](commitment-evidence-review.md) for a shorter test of engineering-source and approval boundaries.
