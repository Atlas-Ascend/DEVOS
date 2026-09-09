# 04 — Architecture

Components: repository adapter, diagnostic engine, patch planner, bounded change executor, test orchestrator, diff/risk summarizer, remediation receipt emitter.

Repair cycle: reproduce -> diagnose -> patch -> local checks -> handoff to independent verification.