# Cumulative Repetition Standard

### Purpose

Every LinuxLabs chapter lab must have two parts:

1. Part 1 - New Chapter Content
2. Part 2 - Cumulative Repetition of All Previous Topics

This prevents the lab series from becoming isolated one-off exercises. Each lab should add new knowledge while also making the learner reuse everything learned so far.

### Core Rule

```text
Every chapter lab = new content + cumulative repetition
```

Part 1 introduces the new material from the current full chapter.

Part 2 repeats and combines all previous topics in a practical operational scenario.

### Full-Chapter Reference Rule

When a book chapter is used as a reference, the whole chapter is the reference unit.

Do not build labs from isolated fragments, short extracts, or individual paragraphs.

Use the full chapter to understand:

* the main topic
* supporting concepts
* warnings and limitations
* command examples
* operational context
* chapter conclusions or summary

The final lab write-up must still be original work and must not copy book material.

### Lab Structure Rule

Every main chapter lab should contain:

```text
Part 1 - New Chapter Content
Part 2 - Cumulative Repetition
```

Both parts should normally be completed on:

* Debian-family system, normally Ubuntu Server LTS
* RHEL-family system, such as RHEL, Rocky Linux, AlmaLinux, or CentOS Stream

### Part 1 - New Chapter Content

Part 1 focuses on the current chapter.

It should include:

* new concepts from the full Practical Linux System Administration chapter
* relevant full-chapter support from other books
* Debian/Ubuntu implementation
* RHEL-family implementation
* Bash or shell usage where relevant
* verification evidence
* distribution comparison

### Part 2 - Cumulative Repetition

Part 2 repeats every topic already learned before the current lab.

It should include:

* at least one task from each previous major topic
* Bash or shell usage
* evidence collection
* post-reboot checks where relevant
* troubleshooting practice where relevant
* Debian/Ubuntu and RHEL-family comparison

### Cumulative Topic Build-Up

| Lab | New topic | Cumulative repetition must include |
| --- | --- | --- |
| 01 | Getting started with Linux | No previous topics; repeat baseline commands until fluent |
| 02 | Permissions and privileged accounts | Lab 01 baseline and CLI checks |
| 03 | User experience and shell environment | Labs 01-02 baseline, CLI, sudo, permissions |
| 04 | Managing users | Labs 01-03 baseline, CLI, sudo, permissions, shell environment |
| 05 | Networking | Labs 01-04 baseline, CLI, sudo, permissions, shell environment, users and groups |
| 06 | Software management | Labs 01-05 plus networking and SSH verification |
| 07 | Storage | Labs 01-06 plus package and network checks |
| 08 | System health | Labs 01-07 plus storage and package checks |
| 09 | Monitoring | Labs 01-08 plus maintenance and health checks |
| 10 | Scripting and automation | Labs 01-09 plus monitoring and maintenance checks |
| 11 | Samba | Labs 01-10 plus Bash automation, storage, users, permissions, networking |
| 12 | Troubleshooting | Labs 01-11 plus service, storage, networking, Samba, Bash evidence |
| 13 | Security | Labs 01-12 plus troubleshooting, logs, services, users, permissions, networking |
| 14 | Continuing education | Labs 01-13 plus knowledge base, scripts, evidence, weak-area review |
| 15 | Making career moves | Labs 01-14 plus full role-readiness review and portfolio evidence |

### Evidence Rule

Part 2 must not be treated as a theory recap.

It must produce practical evidence, such as:

* command output
* config file checks
* service status
* log extracts
* package verification
* filesystem evidence
* user and group evidence
* network checks
* Bash script output
* post-reboot verification

### Documentation Rule

The final write-up should clearly separate:

```text
Part 1 evidence
Part 2 evidence
```

The learner still solves the lab first. Documentation is completed after command output, observations, issues, and seven reflection answers are provided.
