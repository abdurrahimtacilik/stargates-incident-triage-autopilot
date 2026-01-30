# System Architecture

StarGates is designed as an agentic AI system orchestrated by IBM watsonx Orchestrate.

## High-Level Flow

1. User submits an incident alert
2. Sentinel Agent analyzes severity and intent
3. Supporting agents are invoked:
   - Evidence Collector Agent
   - RCA Agent
4. Tools are used to retrieve logs and runbooks
5. Structured outputs are generated

## Why Multi-Agent?

Separating responsibilities:
- Improves reasoning clarity
- Enables auditability
- Mirrors real operational workflows

IBM watsonx Orchestrate manages agent coordination, tool invocation, and response delivery.
