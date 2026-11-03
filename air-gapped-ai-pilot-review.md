# Air-gapped AI pilot acceptance worksheet for semiconductor teams

Published by Tymeline. Use this manual worksheet to run a synthetic engineering workflow inside the intended enclave and record the evidence behind a pilot decision. Scope the checks with the people responsible for the enclave, identity, operations and engineering change control. Keep the completed record and artifacts in the approved environment.

| Review | Exercise | Capture before acceptance |
| --- | --- | --- |
| Local inference and dependencies | With external connectivity unavailable, start the installed system, run an inference and restart it. Exercise the engineering workflow using synthetic input. | Installed build and model versions, the observed behavior, network observation point, any attempted egress and who reviewed it. |
| Local identity and access | Use one authorized reviewer, one unauthorized user and one revoked account. Test the approved workflow and try to approve it with each identity. | Local identity source, role mappings, observed denials and time to apply revocation. |
| Engineering approval | Propose moving a synthetic sample-readiness milestone. Reject it first, then approve a separate proposal as the designated approver. | Original and proposed dates, evidence revision, actor, decision and timestamps. Compare the program record before and after each attempt. |
| Audit and recovery | Reconcile the proposal and both decisions against the local audit record. Restore the supported backup in the approved test environment and check the records again. | Restore scope and version, evidence of what survived, access restrictions and the retention owner. |
| Offline updates | Follow the approved media intake process for a test update. Record integrity verification and exercise the supported recovery procedure. | Package identifier, verification result, custody and approver, and the version and workflow state after recovery. |

## Copyable decision record

- Enclave and permitted interfaces
- Installed application, model and workflow versions
- Acceptance criteria and test evidence references
- Open findings, scope limits and follow-up owners
- Security and engineering decision owners, decisions and dates

A passing run applies to the configuration, interfaces and observation period tested. Set the production acceptance criteria with the enclave owner. [Tymeline's air-gapped AI guide](https://tymeline.ai/resources/air-gapped-ai-semiconductor).
