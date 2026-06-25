# Linux Lab Output Template

Use this template for every LinuxLabs lab. Keep it evidence-based, operational, and production-focused.

---

# Lab Title

## 1. Lab Summary

**Lab:**

**Date completed:**

**Topic area:**

**Difficulty:**

**Status:** Not started / In progress / Completed / Blocked

### Objective

State the purpose of the lab in 2–4 lines.

---

## 2. Scenario

Describe the real-world Linux administration situation this lab simulates.

The scenario should read like a ticket or operational request, not just a tutorial.

---

## 3. Reference Material

| Area | Suggested reference |
| --- | --- |
| Linux command-line usage | The Linux Command Line |
| Modern Linux concepts | Learning Modern Linux |
| Linux administration tasks | Practical Linux System Administration |
| Operating system concepts | Modern Operating Systems |
| Operational thinking | The Practice of System and Network Administration |
| Cloud operations thinking | The Practice of Cloud System Administration |
| RHEL-specific guidance | Red Hat documentation |
| Ubuntu-specific guidance | Ubuntu documentation |

---

## 4. Requirements

| ID | Requirement | Status |
| --- | --- | --- |
| R1 | | Not started |
| R2 | | Not started |
| R3 | | Not started |

---

## 5. Constraints

Record anything you must not do.

Examples:

* Do not disable security controls permanently just to make the lab work.
* Do not commit secrets, SSH private keys, credentials, PDFs, EPUBs, or company data.
* Do not rely on commands you cannot explain.
* Do not mark the lab complete without post-reboot verification.

---

## 6. Assumptions

Record assumptions here.

Examples:

* The lab is performed on both RHEL and Ubuntu unless stated otherwise.
* The systems are disposable lab machines.
* The work must survive a reboot.
* Documentation should be good enough for another engineer to follow.

---

## 7. Expected Lab Structure

Use a structure appropriate for the lab.

Example:

```text
01-linux-foundations/
└── lab-01-build-and-baseline-linux-servers.md
```

---

## 8. Deliverables

| Deliverable | Purpose |
| --- | --- |
| Lab write-up | Records requirements, implementation, evidence, and reflection |
| Verification evidence | Proves the work succeeded |
| RHEL vs Ubuntu notes | Captures distribution differences |
| Break/fix notes | Records troubleshooting and recovery |
| Runbook notes | Captures repeatable operational procedure |

---

## 9. Implementation Tasks

Use these tasks as a guide, not as a full walkthrough.

### Task 1 — Task name

Describe what must be done and what must be proven.

### Task 2 — Task name

Describe what must be done and what must be proven.

### Task 3 — Task name

Describe what must be done and what must be proven.

---

## 10. Key Commands Used

Record important commands only.

| Command | Purpose |
| --- | --- |
| | |
| | |

---

## 11. Files Created or Changed

| Path | Purpose |
| --- | --- |
| | |
| | |

---

## 12. Verification Evidence

This section proves the lab worked.

| Check | Evidence | Result |
| --- | --- | --- |
| | | Passed / Failed |
| | | Passed / Failed |

---

## 13. RHEL vs Ubuntu Comparison

| Area | RHEL | Ubuntu | Notes |
| --- | --- | --- | --- |
| Package management | | | |
| Service management | | | |
| Networking | | | |
| Security controls | | | |
| Logs | | | |
| Config paths | | | |

---

## 14. Break/Fix Scenario

Describe what was deliberately broken or what failure was simulated.

| Failure | Cause | Diagnosis | Fix | Evidence |
| --- | --- | --- | --- | --- |
| | | | | |

---

## 15. Post-Reboot Verification

Nothing counts unless it survives reboot.

| Check | Evidence | Result |
| --- | --- | --- |
| Service/state persisted after reboot | | Passed / Failed |
| Network/storage/security configuration persisted after reboot | | Passed / Failed |
| Documentation updated after final verification | | Passed / Failed |

---

## 16. Diagram

Add a diagram if useful.

If no diagram is required, write:

> No diagram required for this lab.

Example:

```mermaid
flowchart LR
    A[Requirement] --> B[Implementation]
    B --> C[Verification]
    C --> D[Break/Fix]
    D --> E[Post-Reboot Verification]
    E --> F[Documentation]
```

---

## 17. Issues Encountered

| Issue | Cause | Fix |
| --- | --- | --- |
| | | |

If there were no issues, write:

> No major issues encountered.

---

## 18. Decisions Made

| Decision | Reason |
| --- | --- |
| | |
| | |

---

## 19. Security and Production Considerations

Explain the production relevance of the lab.

Cover where relevant:

* access control
* auditability
* rollback and recovery
* repeatability
* least privilege
* reliability
* monitoring
* operational risk
* documentation quality

---

## 20. Final Outcome

State clearly whether the lab was completed.

---

## 21. What I Learned

Write 3–6 bullet points.

---

## 22. What I Would Improve in Production

Write 2–5 bullet points.

---

## 23. References Used

| Reference | Used for |
| --- | --- |
| | |
| | |

---

## 24. Completion Checklist

* [ ] Requirements understood
* [ ] RHEL implementation completed or explicitly marked out of scope
* [ ] Ubuntu implementation completed or explicitly marked out of scope
* [ ] Verification evidence captured
* [ ] RHEL vs Ubuntu comparison completed
* [ ] Break/fix scenario completed
* [ ] Post-reboot verification completed
* [ ] Issues documented
* [ ] Decisions documented
* [ ] Security and production considerations documented
* [ ] Diagram added if useful
* [ ] Work committed with a clear message
* [ ] Work uploaded to the correct topic folder
* [ ] No secrets or private data committed

---

## 25. Reflection Questions

1. What problem did this lab simulate?
2. Which commands mattered most, and why?
3. What differed between RHEL and Ubuntu?
4. What broke, and how did you diagnose it?
5. What evidence proves the final state works?
6. Did the configuration survive reboot?
7. What would be risky about doing this in production?
8. What would you automate next?
9. What would you monitor?
10. What documentation would another engineer need to support this system?
