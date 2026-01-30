
# Evidence Collector Agent

## Role (EN)
The Evidence Collector Agent gathers and summarizes incident evidence to support fast, consistent triage decisions. It focuses on retrieving operational signals (logs/metrics) and extracting the most relevant indicators for downstream root-cause analysis.

## Responsibilities (EN)
- Query logs and metrics using tool calls (mocked for demo where needed)
- Extract key error patterns, spikes, anomalies, and time-correlated signals
- Summarize findings in a structured, enterprise-ready format
- Provide evidence highlights and confidence notes to the RCA Agent

## Inputs (EN)
- service_name
- incident_timestamp / time_window
- suspected_error_pattern (optional)
- runbook_context (optional)

## Outputs (EN)
A structured evidence summary:
- **Evidence Summary:** 3–6 bullet findings
- **Key Signals:** error rates, latency, saturation, dependency failures (as available)
- **Timeline:** what changed and when (relative ordering)
- **Notable Log Snippets:** short, sanitized excerpts (no sensitive data)
- **Confidence & Gaps:** what is known vs. what needs validation

## Tool Usage (EN)
- **Log Query Tool:** retrieves representative logs for the incident window
- **Runbook Retriever Tool (optional):** aligns evidence to known failure modes
- **Ticket Creator Tool (optional):** attaches evidence to the ticket draft payload

## Data & Safety (EN)
- Uses only synthetic or mock data for demonstration
- Avoids personal/sensitive information and sanitizes outputs

---
