# 13 — AI-Assisted Linux Operations

This topic covers responsible AI usage in Linux administration and operations.

### Focus Areas

* AI prompt design for Linux troubleshooting
* command review before execution
* redacted log summarisation
* hypothesis generation during incidents
* runbook and documentation drafting
* RHEL vs Ubuntu comparison support
* safety checks before applying changes
* verification discipline after using AI assistance

### Example Labs

* `lab-01-use-ai-to-review-linux-troubleshooting-plan.md`
* `lab-02-use-ai-to-draft-and-verify-a-linux-runbook.md`
* `lab-03-ai-assisted-log-triage-with-redacted-evidence.md`

### Operational Standard

A lab in this folder should prove that AI was used as an assistant, not as the source of truth.

The final answer must always be proven using real system evidence such as command output, logs, service status, configuration files, and post-reboot verification.

### Safe Use Rules

* Do not paste secrets into AI tools.
* Do not paste private company data into AI tools.
* Redact logs before using AI for summaries.
* Check AI suggestions against official documentation and local system evidence.
* Treat AI-generated commands as drafts until reviewed.
* Record how AI helped and what you independently verified.
