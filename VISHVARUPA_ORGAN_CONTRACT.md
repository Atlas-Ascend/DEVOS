# DEVOS — VISHVARUPA Organ Contract

Status: SEEDED
Organism: VISHVARUPA
Organ class: Software engineering diagnostics / repair / development support

## Mission
DEVOS is the coding and development assistant to the estate build factory. It diagnoses software defects, proposes and applies bounded repairs, validates developer ergonomics, and hands repaired artifacts back into the governed SDLC.

## Authority
May inspect code, generate patches, run bounded development checks, propose migrations, and create remediation packets. May not bypass SECA, self-promote to production, or acquire infrastructure permissions outside assigned scope.

## Inputs
- Packet OS build/repair packets
- MetaForge/VULCAN requests
- CI failures, logs, lint/type/test failures
- runtime defects from Observatory

## Outputs
- patches and repair commits
- diagnostic reports
- test plans
- dependency and migration recommendations
- remediation receipts

## Handoffs
Upstream: Packet-OS, MetaForge, VULCAN, Runtime Observatory, SECA
Downstream: MetaForge/VULCAN, SECA, Release/Deployment Control Plane, ProofGrid

## Events
Consumes: build.failed, test.failed, runtime.defect, remediation.requested
Emits: devos.diagnosed, devos.patch_ready, devos.repair_completed, devos.escalated

## Proof requirements
Every repair identifies defect, causal hypothesis, changed artifact, tests executed, remaining risk, and commit/ref. SECA independently verifies release readiness.

## Definition of integrated
A failing build or runtime defect can become a remediation packet, reach DEVOS, produce a bounded repair, return through SECA, and generate durable proof.