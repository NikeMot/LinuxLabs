# Ansible Mini-Layer

### Purpose

This document defines the lightweight Ansible layer that sits after Bash foundations.

Bash remains the primary learning path for shell fluency. Ansible is introduced to show how repeated Linux administration tasks can be expressed as configuration management.

### Principle

Learn the manual task first.

Then automate it with Bash.

Then express selected tasks in Ansible.

```text
manual Linux skill -> Bash automation -> Ansible representation
```

### Required Scope

The Ansible layer is intentionally small.

The learner should be able to:

* explain what Ansible is used for
* create a simple inventory
* run an ad-hoc command
* write a small playbook
* use `become` safely
* install a package
* manage a service
* copy or template a config file
* create a user or group
* apply a simple file permission change
* compare Bash scripts with Ansible playbooks
* verify changes on both Ubuntu and RHEL-family systems

### Placement

| Area | How Ansible is introduced |
| --- | --- |
| Lab 10 | Convert one Bash maintenance task into an Ansible playbook |
| Lab 12 | Use Ansible ad-hoc commands for evidence gathering where appropriate |
| Lab 13 | Use Ansible to check or apply a small hardening control where appropriate |
| Drill 08 | Optional use of Ansible to rebuild or enforce part of the capstone configuration |

### Example Task Types

Suitable Ansible tasks:

* install `curl` or `nginx`
* ensure a service is enabled and running
* create a local admin group
* deploy a simple config file
* create a directory with correct ownership and mode
* collect facts from both systems

Avoid advanced Ansible until later:

* complex roles
* dynamic inventory
* Ansible Vault
* large multi-role projects
* CI/CD integration
* cloud provisioning

### Evidence Required

For every Ansible exercise, capture:

* inventory used
* command or playbook executed
* changed/ok/failed result
* verification from the target system
* comparison with the manual or Bash approach

### Safety Rule

Do not use Ansible to hide lack of Linux understanding.

The learner must be able to explain what the playbook does on the target system and verify the result with normal Linux commands.
