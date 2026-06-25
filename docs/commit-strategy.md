# Commit Strategy

### Purpose

This document defines how commits should be made in this repository.

The goal is to keep the history readable, reviewable, and safe to revert.

### Commit Principles

Commits should be:

* Small
* Logical
* Complete
* Descriptive
* Safe to revert where possible

### When to Commit

Commit when one logical unit of work is complete.

Examples:

* Creating initial repository structure
* Adding a Linux lab template
* Adding a new lab to the correct topic folder
* Updating verification evidence for one lab
* Fixing a specific documentation error
* Improving one runbook or operational note

### When Not to Commit

Do not commit when:

* Secrets or credentials are present
* Unrelated changes are mixed together
* The change cannot be explained
* The repository is in a broken or confusing state
* The lab contains copied book material instead of original notes
* The lab contains private employer, tenant, customer, or account data

### Commit Message Style

Use short, descriptive messages.

Examples:

* Create Linux lab repository structure
* Add Linux lab output template
* Add build and baseline Linux servers lab
* Document RHEL and Ubuntu service management differences
* Fix storage lab verification checklist

Avoid vague messages such as:

* stuff
* update
* final
* work
* changes

### Pre-Commit Checklist

Before committing:

1. Run `git status`.
2. Review unstaged changes.
3. Review staged changes with `git diff --staged`.
4. Confirm the commit has one clear purpose.
5. Confirm no secrets, private keys, cloud credentials, screenshots, PDFs, EPUBs, or company data are included.
6. Confirm the lab is in the correct numbered topic folder.
7. Confirm the commit message clearly describes the change.

### Branching Rules

Use branches when a change is risky, large, experimental, or separate from the current work on `main`.

Create a branch for:

* a new lab or major documentation update
* changes to repository structure
* experimental work
* anything that may break or confuse the main repository
* work that should be reviewed before merging

Small fixes, such as correcting a typo or improving wording, can be committed directly to `main` while working alone.

In a team or production environment, changes should usually be made on a branch and merged through a pull request.

Branches should have clear names, for example:

```text
docs/update-linux-lab-template
lab/build-baseline-linux-servers
fix/readme-folder-table
```

Delete branches after they have been merged to keep the repository clean.
