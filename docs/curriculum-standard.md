# Linux Curriculum Standard

## Curriculum Spine

The LinuxLabs programme uses two primary books only:

1. **How Linux Works, 3rd Edition** by Brian Ward
2. **The Linux Command Line, 3rd Edition** by William Shotts

Each normal lab combines:

* 1 chapter from **How Linux Works**
* 2 chapters from **The Linux Command Line**
* official documentation relevant to the lab topic
* one focused operational scenario
* one evidence-driven verification outcome
* one controlled break/fix element where practical

## Lab Count

The programme is organised as:

* **17 standard labs**
* **1 final capstone lab**
* **18 labs total**

This works because **How Linux Works** has 17 chapters and **The Linux Command Line** has 36 chapters.

The first 17 labs map one **How Linux Works** chapter to two **The Linux Command Line** chapters.

The final two **The Linux Command Line** chapters are handled in the capstone.

## Duration Rule

Each standard lab must be scoped for **60–90 minutes maximum** of active learner work.

If a lab cannot realistically fit inside 90 minutes, split the lab rather than increasing the duration.

The capstone may be larger than a standard lab, but it should still be broken into clear phases so it does not become vague or unmanageable.

## Official Documentation Requirement

Every lab must include an official documentation check.

Use official documentation to confirm current behaviour, commands, service names, configuration paths, package names, security controls, and version-specific differences.

Suitable sources include:

* Red Hat documentation
* Ubuntu Server documentation
* Debian documentation where relevant
* GNU Bash manual
* GNU Coreutils manual
* systemd documentation and local man pages
* OpenSSH documentation
* firewalld documentation
* Netplan documentation
* package documentation installed on the local system
* command help and local man pages

AI output is not official documentation and is not verification evidence.

## Normal Lab Pattern

Each standard lab should follow this pattern:

1. Read the assigned **How Linux Works** chapter.
2. Read the assigned two **The Linux Command Line** chapters.
3. Check official documentation relevant to the scenario.
4. Solve the operational lab.
5. Capture command output, observations, issues, and verification evidence.
6. Answer exactly seven reflection questions.
7. Final documentation and GitHub upload are completed after the learner provides evidence and reflection answers.

## Capstone Pattern

The final capstone should integrate the full programme.

It should include:

* Linux system investigation
* command-line fluency
* shell scripting
* users, groups, permissions, and sudo
* software/package management
* systemd and services
* logging and troubleshooting
* networking and SSH
* storage/filesystem checks
* security and hardening basics
* backup or recovery thinking
* automation with Bash
* official documentation validation
* controlled break/fix
* post-reboot verification
* final operational runbook

The capstone should use the final two **The Linux Command Line** chapters and force practical reuse of the earlier Linux topics.

## Documentation Rule

The final lab write-up must record:

* assigned book chapters
* official documentation checked
* commands used
* files created or changed
* verification evidence
* issues encountered
* decisions made
* break/fix evidence
* security and production considerations
* seven reflection answers

The learner solves the lab. Documentation, formatting, evidence organisation, and repository upload are handled separately.
