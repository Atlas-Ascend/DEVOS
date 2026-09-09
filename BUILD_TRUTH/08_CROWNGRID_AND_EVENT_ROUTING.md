# 08 — CrownGrid and Event Routing

Consumes: build.failed, test.failed, runtime.defect, remediation.requested, packet.routed.
Emits: devos.diagnosed, devos.patch_planned, devos.patch_ready, devos.repair_completed, devos.escalated.

CrownGrid routes to DEVOS when requested software-engineering capabilities and permissions match.