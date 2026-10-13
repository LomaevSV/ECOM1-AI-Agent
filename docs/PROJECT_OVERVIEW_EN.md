# ECOM1 project overview

[Русский](PROJECT_OVERVIEW_RU.md) · [Home](../README_EN.md)

## Purpose and scenarios

ECOM1 processes tasks in the BitGN e-commerce tool environment. Code-supported paths include attribute-based product lookup, inventory and count queries, policy decisions, evidence-linked answers, and a specialized archived-payment investigation.

## Current state

The snapshot contains a CLI entry point, environment connectors, an LLM client, orchestrator, executor, retrieval, deterministic handlers, and memory. Presence in code does not establish successful operation: no external benchmark run was performed and the included test suite does not pass. See the audit.

## Engineering approach

The implementation separates policy decisions from general task execution; uses structured intents, attribute scoring, tool-derived evidence references, an answer contract, bounded repair attempts, and dedicated model roles. Episodic memory is process-local, not a verified durable database.

## Scope and limitations

The agent is tied to a benchmark tool interface and its data model. Production deployment, scalability, operational SLAs, and comprehensive adversarial robustness are not demonstrated.

## Public scope and next steps

Only architecture documentation is released. Source and environment data remain private. Reproducible regression testing and unified candidate selection remain future work.
