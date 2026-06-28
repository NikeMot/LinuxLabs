# Linux Lab Output Template

Use this template for every LinuxLabs lab. Keep it evidence-based, operational, current, and production-focused.

The learner should focus on solving the lab. Documentation, formatting, evidence organisation, and GitHub upload are handled after the learner provides command output, observations, issues encountered, and answers to the seven reflection questions.

Every applicable lab must be attempted on both a Debian-family system, normally Ubuntu Server LTS, and a RHEL-family system. A lab is not complete until both implementations have evidence, unless one family is explicitly marked out of scope with a reason.

Every chapter lab has two parts:

1. **Part 1 — New Chapter Content**
2. **Part 2 — Cumulative Repetition of All Previous Topics**

Every lab must include controlled break/fix practice.

```text
No break/fix = lab not complete.
```

Every lab must include an online documentation check.

```text
No current documentation check = lab not complete.
```

When a book chapter is used as a reference, use the full chapter as the reference unit, not isolated extracts.

---

# Lab Title

## 1. Lab Summary

**Lab:**

**Date completed:**

**Topic area:**

**Difficulty:**

**Status:** Not started / In progress / Completed / Blocked

**Debian/Ubuntu status:** Not started / In progress / Completed / Out of scope

**RHEL-family status:** Not started / In progress / Completed / Out of scope

**Break/fix status:** Not started / In progress / Completed / Blocked

**Online documentation check:** Not started / Completed / Not applicable with reason

### Objective

State the purpose of the lab in 2–4 lines.

---

## 2. Scenario

Describe the real-world Linux administration situation this lab simulates.

The scenario should read like a ticket or operational request, not just a tutorial.

---

## 3. Reference Material

| Area | Suggested reference | Chapter or documentation usage |
| --- | --- | --- |
| Linux command-line usage | The Linux Command Line | Use full relevant chapter |
| Modern Linux concepts | Learning Modern Linux | Use full relevant chapter |
| Linux administration tasks | Practical Linux System Administration | Use full current chapter |
| Operating system concepts | Modern Operating Systems / Operating System Concepts | Use full relevant chapter |
| Operational thinking | The Practice of System and Network Administration | Use full relevant chapter or section-level operational principle only where no chapter mapping exists |
| Cloud operations thinking | The Practice of Cloud System Administration | Use full relevant chapter where used |
| RHEL-specific guidance | Red Hat documentation | Use current official task guidance |
| Ubuntu-specific guidance | Ubuntu Server documentation | Use current official task guidance |
| Debian-family guidance | Debian documentation | Use current official task guidance where relevant |
| systemd | systemd documentation and local man pages | Use current project docs and installed-system man pages |
| Ansible | Ansible documentation | Use documentation matching installed Ansible version |
| Samba/NFS/OpenSSH | Official project or vendor documentation | Use current official documentation |
| Local system documentation | man pages, package docs, command help | Use installed-system truth |
| AI-assisted operations | Lab notes, official product documentation, and verified system evidence | AI is not evidence |

---

## 4. Online Documentation Check

Use this section to prove current documentation was checked before relying on commands, package names, service names, config paths, firewall behaviour, or security controls.

| Source used | Topic checked | Date checked | Version/distribution | Lab decision affected |
| --- | --- | --- | --- | --- |
| | | | | |
| | | | | |

### Documentation Notes

Record any important version-specific findings.

Examples:

* Ubuntu service name differed from RHEL-family service name.
* Red Hat guidance used firewalld rather than ufw.
* Local man page confirmed the option used in this lab.
* Package name differed between `apt` and `dnf`.

---

## 5. Requirements

| ID | Requirement | Debian/Ubuntu status | RHEL-family status |
| --- | --- | --- | --- |
| R1 | | Not started | Not started |
| R2 | | Not started | Not started |
| R3 | | Not started | Not started |

---

## 6. Constraints

Record anything the learner must not do.

Examples:

* Do not disable security controls permanently just to make the lab work.
* Do not commit secrets, SSH private keys, credentials, PDFs, EPUBs, or company data.
* Do not rely on commands that cannot be explained.
* Do not mark the lab complete without post-reboot verification.
* Do not treat AI output as proof without local verification.
* Do not mark a lab complete if only one distribution family has been attempted, unless the other is explicitly out of scope with a reason.
* Do not mark a lab complete without controlled break/fix practice.
* Do not mark a lab complete without checking current documentation where implementation details could change.
* Do not perform break/fix on employer, production, shared, or sensitive systems.
* Do not use isolated book extracts as the lab reference when a full chapter is available.
* Do not copy large sections of online documentation into the repository.

---

## 7. Assumptions

Record assumptions here.

Examples:

* The lab is performed on both Debian/Ubuntu and RHEL-family systems unless stated otherwise.
* The systems are disposable lab machines.
* The work must survive a reboot.
* Documentation should be good enough for another engineer to follow.
* Part 2 repeats all topics previously learned in the series.
* Break/fix work is performed only after a baseline state or snapshot exists.
* Official online documentation and local man pages are used to confirm current implementation details.

---

## 8. Expected Lab Structure

Use a structure appropriate for the lab.

Example:

```text
01-getting-started-with-linux/
└── lab-01-bootstrap-and-baseline-linux-server.md
```

---

## 9. Deliverables

| Deliverable | Purpose |
| --- | --- |
| Lab write-up | Records requirements, implementation, evidence, and reflection |
| Online documentation check | Proves current official/local documentation was checked |
| Part 1 evidence | Proves the new chapter content was completed |
| Part 2 evidence | Proves previous topics were repeated and combined |
| Debian/Ubuntu evidence | Proves the work succeeded on Ubuntu or another Debian-family system |
| RHEL-family evidence | Proves the work succeeded on RHEL, Rocky, AlmaLinux, or CentOS Stream |
| RHEL vs Ubuntu notes | Captures distribution differences |
| Break/fix evidence | Proves baseline, failure, diagnosis, fix, recovery, and prevention |
| AI-assisted operations notes | Records where AI helped and what was verified independently |
| Runbook notes | Captures repeatable operational procedure |

---

## 10. Part 1 — New Chapter Content

Part 1 focuses on the current full chapter.

### New Content Tasks

| Task | Debian/Ubuntu requirement | RHEL-family requirement | Evidence required |
| --- | --- | --- | --- |
| Task 1 | | | |
| Task 2 | | | |
| Task 3 | | | |

### Part 1 Break/Fix

Where practical, include a controlled failure related to the new chapter content.

| Failure | Debian/Ubuntu task | RHEL-family task | Recovery evidence |
| --- | --- | --- | --- |
| | | | |

### Part 1 Evidence

| Check | Debian/Ubuntu evidence | RHEL-family evidence | Result |
| --- | --- | --- | --- |
| | | | Passed / Failed |
| | | | Passed / Failed |

---

## 11. Part 2 — Cumulative Repetition of All Previous Topics

Part 2 repeats all topics learned before this lab.

For Lab 01, repeat the baseline checks until fluent.

For Lab 02 onward, include practical repetition from every earlier lab.

### Previous Topics to Repeat

| Previous lab/topic | Debian/Ubuntu task | RHEL-family task | Evidence required |
| --- | --- | --- | --- |
| Lab 01 baseline/CLI | | | |
| Lab 02 permissions/sudo | | | |
| Lab 03 shell environment | | | |
| Lab 04 users/groups | | | |
| Lab 05 networking/SSH | | | |
| Lab 06 software/packages | | | |
| Lab 07 storage/filesystems | | | |
| Lab 08 system health | | | |
| Lab 09 monitoring/performance | | | |
| Lab 10 scripting/automation | | | |
| Lab 11 Samba/file sharing | | | |
| Lab 12 troubleshooting | | | |
| Lab 13 security | | | |
| Lab 14 learning system | | | |

Remove rows that are not yet applicable.

### Part 2 Break/Fix

From Lab 05 onward, Part 2 should include its own cumulative break/fix scenario where practical.

| Failure | Previous topics involved | Debian/Ubuntu task | RHEL-family task | Recovery evidence |
| --- | --- | --- | --- | --- |
| | | | | |

### Part 2 Evidence

| Check | Debian/Ubuntu evidence | RHEL-family evidence | Result |
| --- | --- | --- | --- |
| | | | Passed / Failed |
| | | | Passed / Failed |

---

## 12. Key Commands Used

Record important commands only.

| Command | Part | Debian/Ubuntu purpose | RHEL-family purpose | Documentation checked |
| --- | --- | --- | --- | --- |
| | Part 1 / Part 2 / Break-Fix | | | |
| | Part 1 / Part 2 / Break-Fix | | | |

---

## 13. Files Created or Changed

| Path | Part | Debian/Ubuntu | RHEL-family | Purpose | Documentation checked |
| --- | --- | --- | --- | --- | --- |
| | Part 1 / Part 2 / Break-Fix | | | | |
| | Part 1 / Part 2 / Break-Fix | | | | |

---

## 14. Debian/Ubuntu Implementation Evidence

This section proves the lab worked on Ubuntu or another Debian-family system.

| Check | Part | Evidence | Result |
| --- | --- | --- | --- |
| | Part 1 / Part 2 / Break-Fix | | Passed / Failed |
| | Part 1 / Part 2 / Break-Fix | | Passed / Failed |

---

## 15. RHEL-Family Implementation Evidence

This section proves the lab worked on RHEL, Rocky Linux, AlmaLinux, or CentOS Stream.

| Check | Part | Evidence | Result |
| --- | --- | --- | --- |
| | Part 1 / Part 2 / Break-Fix | | Passed / Failed |
| | Part 1 / Part 2 / Break-Fix | | Passed / Failed |

---

## 16. RHEL vs Ubuntu Comparison

| Area | RHEL-family | Debian/Ubuntu | Notes |
| --- | --- | --- | --- |
| Package management | | | |
| Service management | | | |
| Networking | | | |
| Security controls | | | |
| Logs | | | |
| Config paths | | | |
| Filesystems/storage | | | |
| Shell/user environment | | | |
| Break/fix diagnosis | | | |
| Documentation source | | | |

---

## 17. Mandatory Break/Fix Scenario

No lab is complete without this section.

Minimum requirement:

```text
At least one controlled break/fix scenario per lab.
```

Preferred from Lab 05 onward:

```text
One break/fix scenario in Part 1 and one break/fix scenario in Part 2.
```

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
| Post-reboot evidence where relevant | |
| Prevention note | |

### Break/Fix Summary

| Failure | Part | Family affected | Cause | Diagnosis | Fix | Evidence |
| --- | --- | --- | --- | --- | --- | --- |
| | Part 1 / Part 2 | Debian/Ubuntu / RHEL-family / Both | | | | |

---

## 18. Post-Reboot Verification

Nothing counts unless it survives reboot.

| Check | Part | Debian/Ubuntu evidence | RHEL-family evidence | Result |
| --- | --- | --- | --- | --- |
| Service/state persisted after reboot | Part 1 / Part 2 / Break-Fix | | | Passed / Failed |
| Network/storage/security configuration persisted after reboot | Part 1 / Part 2 / Break-Fix | | | Passed / Failed |
| Documentation updated after final verification | Part 1 / Part 2 / Break-Fix | | | Passed / Failed |

---

## 19. AI-Assisted Operations Notes

Use this section when AI was used during the lab.

| AI use | Part | What it helped with | What was independently verified | Evidence |
| --- | --- | --- | --- | --- |
| | Part 1 / Part 2 / Break-Fix | | | |

If AI was not used, write:

> AI was not used for this lab.

---

## 20. Diagram

Add a diagram if useful.

If no diagram is required, write:

> No diagram required for this lab.

---

## 21. Issues Encountered

| Issue | Part | Family affected | Cause | Fix |
| --- | --- | --- | --- | --- |
| | Part 1 / Part 2 / Break-Fix | | | |

If there were no issues, write:

> No major issues encountered.

---

## 22. Decisions Made

| Decision | Part | Reason | Documentation or evidence used |
| --- | --- | --- | --- |
| | Part 1 / Part 2 / Break-Fix | | |
| | Part 1 / Part 2 / Break-Fix | | |

---

## 23. Security and Production Considerations

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
* distro differences
* current documentation checked
* responsible AI usage
* cumulative repetition and skill retention
* what would prevent the break/fix issue recurring in production

---

## 24. Final Outcome

State clearly whether Part 1, Part 2, the mandatory break/fix scenario, and the online documentation check were completed on both Debian/Ubuntu and RHEL-family systems.

---

## 25. What I Learned

Summarise the learner's reflection answers into 3–6 bullet points.

---

## 26. What I Would Improve in Production

Summarise production improvements from the learner's reflection answers.

---

## 27. References Used

| Reference | Chapter/documentation used | Used for | Date checked |
| --- | --- | --- | --- |
| | Full chapter / official guidance / local man page | | |
| | Full chapter / official guidance / local man page | | |

---

## 28. Completion Checklist

* [ ] Requirements understood
* [ ] Part 1 new chapter content completed
* [ ] Part 2 cumulative repetition completed
* [ ] Full chapter used where a book chapter was referenced
* [ ] Online documentation checked where implementation details could change
* [ ] Local man pages or package documentation checked where relevant
* [ ] Debian/Ubuntu implementation completed or explicitly marked out of scope with a reason
* [ ] RHEL-family implementation completed or explicitly marked out of scope with a reason
* [ ] Debian/Ubuntu verification evidence captured
* [ ] RHEL-family verification evidence captured
* [ ] RHEL vs Ubuntu comparison completed
* [ ] Mandatory break/fix scenario completed
* [ ] Break/fix baseline captured
* [ ] Break/fix symptoms captured
* [ ] Break/fix diagnosis captured
* [ ] Break/fix fix captured
* [ ] Break/fix recovery evidence captured
* [ ] Break/fix prevention note captured
* [ ] Post-reboot verification completed for both applicable families
* [ ] AI-assisted operations notes completed or marked not used
* [ ] Issues documented
* [ ] Decisions documented
* [ ] Security and production considerations documented
* [ ] Diagram added if useful
* [ ] Seven reflection answers captured
* [ ] Work committed with a clear message
* [ ] Work uploaded to the correct topic folder
* [ ] No secrets or private data committed

---

## 29. Reflection Questions

Ask exactly seven reflection questions at the end of the lab.

1. What problem did this lab simulate?
2. What new chapter content did you practise, and what previous topics did Part 2 force you to repeat?
3. What did you deliberately break or diagnose, and what evidence led you to the fix?
4. What current documentation or local man pages did you check, and what decision did they affect?
5. What evidence proves your solution worked on both Debian/Ubuntu and RHEL-family systems?
6. Where did AI help, if at all, and what did you verify yourself?
7. What would you improve, automate, or monitor next time?
