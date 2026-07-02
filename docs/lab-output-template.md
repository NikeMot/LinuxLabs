# Linux Lab Output Template

Use this template for every LinuxLabs lab.

The programme uses a simple two-book spine:

1. **How Linux Works, 3rd Edition** — one chapter per standard lab
2. **The Linux Command Line, 3rd Edition** — two chapters per standard lab

Every standard lab must include official documentation checks, practical verification evidence, and a controlled break/fix element where practical.

The learner should focus on solving the lab. Documentation, formatting, evidence organisation, and GitHub upload are handled after the learner provides command output, observations, issues encountered, and answers to the seven reflection questions.

---

# Lab Title

## 1. Lab Summary

**Lab:**

**Estimated duration:** 60–90 minutes maximum

**Actual duration:**

**Topic area:**

**Difficulty:**

**Status:** Not started / In progress / Completed / Blocked

**Break/fix status:** Not started / In progress / Completed / Blocked

**Official documentation check:** Not started / Completed / Not applicable with reason

### Objective

State the purpose of the lab in 2–4 lines.

---

## 2. Chapter Mapping

| Source | Chapter(s) | Used for |
| --- | --- | --- |
| How Linux Works, 3rd Edition | Chapter X | Linux system concept for this lab |
| The Linux Command Line, 3rd Edition | Chapters X–Y | Shell, command-line, or Bash automation practice |
| Official documentation | Product/vendor/local docs checked | Current implementation details |

---

## 3. Scenario

Describe the real-world Linux administration situation this lab simulates.

The scenario should read like a ticket or operational request, not just a tutorial.

---

## 4. Official Documentation Check

Use this section to prove current documentation was checked before relying on commands, package names, service names, config paths, firewall behaviour, security controls, or shell behaviour.

| Source used | Topic checked | Date checked | Version/distribution | Lab decision affected |
| --- | --- | --- | --- | --- |
| | | | | |
| | | | | |

Suitable sources include Red Hat documentation, Ubuntu Server documentation, Debian documentation, GNU Bash manual, GNU Coreutils manual, systemd documentation, OpenSSH documentation, firewalld documentation, Netplan documentation, command help, local man pages, and installed package documentation.

AI output is not official documentation and is not verification evidence.

---

## 5. Requirements

| ID | Requirement | Status |
| --- | --- | --- |
| R1 | | Not started |
| R2 | | Not started |
| R3 | | Not started |

---

## 6. Constraints

Record anything the learner must not do.

Examples:

* Do not commit secrets, SSH private keys, credentials, PDFs, EPUBs, or company data.
* Do not rely on commands that cannot be explained.
* Do not mark the lab complete without verification evidence.
* Do not treat AI output as proof without local verification.
* Do not perform break/fix on employer, production, shared, or sensitive systems.
* Do not copy large sections of book or online documentation into the repository.
* Do not let the active solving portion exceed 90 minutes; split the lab if needed.

---

## 7. Assumptions

Record assumptions here.

Examples:

* The system is a disposable lab machine.
* The learner has snapshot, rollback, or rebuild options.
* The work should survive a reboot where persistence matters.
* Official documentation and local man pages are used to confirm current implementation details.
* The lab is scoped for 60–90 minutes of active learner work.

---

## 8. Expected Lab Structure

Use a structure appropriate for the lab.

Example:

```text
01-linux-foundations/
└── lab-01-bootstrap-and-baseline-linux-server.md
```

---

## 9. Deliverables

| Deliverable | Purpose |
| --- | --- |
| Lab write-up | Records requirements, implementation, evidence, and reflection |
| Official documentation check | Proves current official/local documentation was checked |
| Command output | Proves what was run and observed |
| Verification evidence | Proves the solution worked |
| Break/fix evidence | Proves baseline, failure, diagnosis, fix, recovery, and prevention |
| AI-assisted operations notes | Records where AI helped and what was verified independently |
| Runbook notes | Captures repeatable operational procedure where useful |

---

## 10. Implementation Tasks

The learner solves the lab. Final documentation is completed after the learner provides evidence and reflection answers.

| Task | Requirement | Evidence required | Status |
| --- | --- | --- | --- |
| Task 1 | | | Not started |
| Task 2 | | | Not started |
| Task 3 | | | Not started |

---

## 11. Key Commands Used

Record important commands only.

| Command | Purpose | Documentation checked |
| --- | --- | --- |
| | | |
| | | |

---

## 12. Files Created or Changed

| Path | Purpose | Documentation checked |
| --- | --- | --- |
| | | |
| | | |

---

## 13. Verification Evidence

| Check | Evidence | Result |
| --- | --- | --- |
| | | Passed / Failed |
| | | Passed / Failed |

---

## 14. Mandatory Break/Fix Scenario

Every lab should include one controlled break/fix element where practical.

If break/fix is not practical for a specific lab, record why.

### Break/Fix Evidence

| Stage | Evidence |
| --- | --- |
| Baseline | |
| Controlled failure introduced or encountered | |
| Symptoms observed | |
| Diagnostic commands used | |
| Likely or confirmed cause | |
| Documentation checked | |
| Fix applied | |
| Recovery evidence | |
| Prevention note | |

---

## 15. Post-Reboot Verification

Use this section where persistence matters.

| Check | Evidence | Result |
| --- | --- | --- |
| Service/state persisted after reboot | | Passed / Failed / Not applicable |
| Network/storage/security configuration persisted after reboot | | Passed / Failed / Not applicable |
| Documentation updated after final verification | | Passed / Failed |

---

## 16. AI-Assisted Operations Notes

Use this section when AI was used during the lab.

| AI use | What it helped with | What was independently verified | Evidence |
| --- | --- | --- | --- |
| | | | |

If AI was not used, write:

> AI was not used for this lab.

---

## 17. Issues Encountered

| Issue | Cause | Fix |
| --- | --- | --- |
| | | |

If there were no issues, write:

> No major issues encountered.

---

## 18. Decisions Made

| Decision | Reason | Documentation or evidence used |
| --- | --- | --- |
| | | |
| | | |

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
* current documentation checked
* responsible AI usage
* what would prevent the break/fix issue recurring in production

---

## 20. Final Outcome

State clearly whether the requirements, official documentation check, verification evidence, and break/fix element were completed.

---

## 21. What I Learned

Summarise the learner's reflection answers into 3–6 bullet points.

---

## 22. What I Would Improve in Production

Summarise production improvements from the learner's reflection answers.

---

## 23. References Used

| Reference | Chapter/documentation used | Used for | Date checked |
| --- | --- | --- | --- |
| How Linux Works, 3rd Edition | Chapter X | Linux concept | |
| The Linux Command Line, 3rd Edition | Chapters X–Y | Shell/command-line practice | |
| Official documentation | | Current implementation details | |

---

## 24. Completion Checklist

* [ ] Estimated duration is 60–90 minutes maximum
* [ ] One How Linux Works chapter assigned
* [ ] Two The Linux Command Line chapters assigned
* [ ] Official documentation checked where implementation details could change
* [ ] Requirements understood
* [ ] Implementation completed
* [ ] Command output captured
* [ ] Verification evidence captured
* [ ] Break/fix completed or explicitly marked not practical with a reason
* [ ] Post-reboot verification completed where relevant
* [ ] AI-assisted operations notes completed or marked not used
* [ ] Issues documented
* [ ] Decisions documented
* [ ] Security and production considerations documented
* [ ] Seven reflection answers captured
* [ ] Work committed with a clear message
* [ ] Work uploaded to the correct topic folder
* [ ] No secrets or private data committed

---

## 25. Seven Reflection Questions

Ask exactly seven reflection questions at the end of the lab:

1. What problem did this lab simulate?
2. What commands, files, or services mattered most in solving it?
3. What evidence proves your solution worked?
4. What broke, confused you, or required troubleshooting?
5. What would be risky about doing this in production?
6. Where did AI help, if at all, and what did you verify yourself?
7. What would you improve, automate, or monitor next time?
