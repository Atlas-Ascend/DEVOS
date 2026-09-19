# ARK Ω Runtime Binding v1.1.0 — DEVOS

Role: delivery/runtime verification gate after SECA.

Consume only SECA PASS receipts with preserved command_id, mission_id and packet_id. Validate deployability/runtime health, artifact integrity, rollback metadata and delivery-state consistency.

Required transition: VERIFYING -> VERIFIED_FOR_PROOF.

Emit devos_receipt with verdict PASS|FAIL|WITHHELD, runtime_checks[], deployment_refs[], rollback_ref, artifact_hashes[], timestamp and correlation ids.

Any non-PASS result blocks ProofGrid sealing and must return to ARK Ω as FAILED/WITHHELD.
