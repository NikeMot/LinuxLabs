# LinuxLabs

### Overview

The LinuxLabs repository contains my hands-on Linux system administration labs aimed at developing practical Linux, infrastructure, SRE operations, and AI-assisted operations skills.

The canonical LinuxLabs programme is now a **15-lab chapter-led series** based on *Practical Linux System Administration* by Kenneth Hess. Each lab maps to one chapter of that book and expands it with material from the other Linux and operating systems books in my Drive.

The goal is not just to learn commands, but to build production-style operational judgement: build, verify, troubleshoot, document, recover, compare distributions, use AI responsibly, and explain decisions.

### Core Rule

One chapter equals one lab.

```text
15 chapters = 15 labs
```

By the end of Lab 15, the LinuxLabs series should have covered the practical administration content from *Practical Linux System Administration* and the relevant supporting concepts from the other Linux, operating systems, cloud administration, and system administration books.

### Primary Reference

| Role | Reference |
| --- | --- |
| Main lab sequence | Practical Linux System Administration |
| Execution standard | The Practice of System and Network Administration |
| Cloud operations mindset | The Practice of Cloud System Administration |
| Command-line depth | The Linux Command Line |
| Modern Linux depth | Learning Modern Linux |
| Operating system theory | Modern Operating Systems / Operating System Concepts |
| AI support | Responsible AI-assisted operations notes and verified system evidence |

### Lab Series

| Lab | Folder | Practical Linux chapter | Status |
| --- | --- | --- | --- |
| 01 | `01-getting-started-with-linux/` | Getting Started with Linux | Not started |
| 02 | `02-working-with-permissions-and-privileged-accounts/` | Working with Permissions and Privileged Accounts | Not started |
| 03 | `03-customizing-the-user-experience/` | Customizing the User Experience | Not started |
| 04 | `04-managing-users/` | Managing Users | Not started |
| 05 | `05-connecting-to-a-network/` | Connecting to a Network | Not started |
| 06 | `06-installing-and-uninstalling-software/` | Installing and Uninstalling Software | Not started |
| 07 | `07-managing-storage/` | Managing Storage | Not started |
| 08 | `08-maintaining-system-health/` | Maintaining System Health | Not started |
| 09 | `09-monitoring-your-system/` | Monitoring Your System | Not started |
| 10 | `10-scripting-and-automation/` | Scripting and Automation | Not started |
| 11 | `11-deploying-samba-for-windows-compatibility/` | Deploying Samba for Windows Compatibility | Not started |
| 12 | `12-troubleshooting-linux/` | Troubleshooting Linux | Not started |
| 13 | `13-securing-your-system/` | Securing Your System | Not started |
| 14 | `14-continuing-your-education/` | Continuing Your Education | Not started |
| 15 | `15-making-career-moves/` | Making Career Moves | Not started |

### Naming Convention

Topic folders use this format:

```text
01-topic-name-written-lowercase
```

Lab files inside topic folders use this format:

```text
lab-01-short-lab-title.md
```

Example:

```text
01-getting-started-with-linux/lab-01-bootstrap-and-baseline-linux-server.md
```

### How to Use This Repository

Each lab should include:

* Scenario
* Reference material
* Requirements
* Constraints
* Assumptions
* Implementation tasks
* Key commands used
* Files created or changed
* Verification evidence
* RHEL vs Ubuntu comparison, where relevant
* Break/fix scenario
* Post-reboot verification
* AI-assisted operations notes, where relevant
* Issues encountered
* Decisions made
* Security and production considerations
* Final outcome
* What I learned
* What I would improve in production
* References used
* Completion checklist
* Seven reflection questions

### Learner Workflow

The learner solves the lab. Documentation, formatting, evidence organisation, and GitHub upload are handled after the lab is solved.

The learner provides command output, observations, issues, final verification evidence, and answers to seven reflection questions.

### Security and Privacy Notes

The repository must not contain:

* Passwords
* API keys
* SSH private keys
* `.env` files
* Cloud credentials
* Company data
* Screenshots containing private tenant, account, or user information
* Book PDFs or EPUBs
* Copyrighted training material
* Sensitive logs
* Private IP addressing or hostnames from a real employer environment

### AI Usage Rule

AI may be used as a learning and operations assistant, but it must not replace verification.

Use AI for explanation, planning, command review, log summaries, runbook drafts, comparison notes, and checklists. Always validate AI suggestions with real command output, logs, documentation, and post-reboot testing.

### Lab Upload Rule

Every new Linux lab must be committed to the correct numbered chapter folder. Labs should not be placed at the repository root.
