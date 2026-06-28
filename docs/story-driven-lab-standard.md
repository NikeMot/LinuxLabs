# Story-Driven Lab Standard

### Purpose

Every LinuxLabs lab must have a story and an operational reason.

The learner should never feel as if they are only typing commands. Commands must exist inside a realistic situation: a request, incident, change, audit, recovery task, support ticket, or production-readiness exercise.

### Core Rule

```text
No story = no lab.
No operational reason = no command.
```

A lab must explain:

* who is asking for the work
* what system or service is affected
* why the work matters
* what risk exists if the work is done badly
* what evidence proves the work succeeded
* how the work relates to real Linux administration, infrastructure, SRE, or support practice

### Required Lab Shape

Every lab must include:

1. Lab summary
2. Story-driven scenario
3. Manager, team, customer, or incident-style requirement
4. Reference material
5. Online documentation check
6. Requirements
7. Constraints
8. Assumptions
9. Part 1 - New Chapter Content
10. Part 2 - Cumulative Repetition of All Previous Topics
11. Mandatory break/fix scenario
12. Evidence and verification
13. Decisions made
14. Issues encountered
15. Security and production considerations
16. Final outcome
17. Reflection questions

### Scenario Standard

The scenario must read like real work.

Good scenario patterns:

* a manager asks for a system to be prepared
* a service owner reports a failure
* a security review finds a weakness
* a team needs a repeatable operating procedure
* a platform team needs a baseline before deploying services
* a user or application team cannot access something
* a change must be completed safely and documented
* an incident must be diagnosed and recovered

Bad scenario patterns:

* "Run these commands"
* "Practise command X"
* "Install package Y"
* "Learn topic Z"

Those can be tasks inside the lab, but they are not enough to justify the lab.

### Manager Requirement Standard

Every lab should contain a short requirement written like a real operational instruction.

Example format:

```text
Your manager gives you this requirement:

> Prepare this Linux host so it can be supported by another engineer. Do not just install tools. Prove the system is reachable, documented, recoverable, and safe to continue building on.
```

The requirement should explain the business or operational reason behind the work.

### Command Justification Rule

Every important command should answer at least one of these questions:

* What am I trying to prove?
* What am I trying to change?
* What failure am I investigating?
* What risk am I reducing?
* What evidence am I collecting?
* What decision will this output support?

If a command has no reason, it does not belong in the lab.

### Break/Fix Story Rule

The break/fix section must also have a story.

Do not only say:

```text
Break SSH and fix it.
```

Prefer:

```text
A developer reports that they cannot connect to the host after a hardening change. You must confirm whether the issue is authentication, service state, firewall policy, or configuration, then restore access without weakening the final security posture.
```

### Evidence Story Rule

Evidence should show progress through the story.

Good evidence answers:

* What was the starting state?
* What changed?
* What broke?
* What symptom appeared?
* What did the logs or commands prove?
* What fixed the issue?
* What proves the system is safe after reboot?

### Reflection Rule

The reflection questions should help the learner explain the operational story, not only define commands.

The learner should be able to answer:

* why the work mattered
* what problem was being solved
* what was deliberately broken or diagnosed
* what evidence mattered
* what would be risky in production
* what would be improved, automated, monitored, or documented next

### Completion Standard

A lab is complete only when the final write-up makes the work understandable to another engineer who did not watch the learner perform the commands.

The final lab should read like evidence of operational judgement, not a command transcript.
