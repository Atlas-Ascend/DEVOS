# 05 — Interfaces and Schemas

RepairRequest: packet_id, repo/ref, defect, logs/evidence, allowed_paths, constraints, acceptance_criteria.

RepairResult: hypothesis, changed_paths, commit/diff ref, tests_run, results, unresolved_risk, followups, verification_request.