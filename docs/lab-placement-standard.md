# Lab Placement Standard

### Purpose

Every LinuxLabs lab must be placed in the correct numbered chapter folder.

The canonical lab series follows the 15 chapters of *Practical Linux System Administration*.

### Folder Naming

Use this format:

```text
01-topic-name-written-lowercase
```

Rules:

* use two-digit numbering
* use lowercase words
* separate words with hyphens
* align the folder with the Practical Linux chapter title
* do not place labs at the repository root

### Lab File Naming

Use this format:

```text
lab-01-short-lab-title.md
```

Example:

```text
01-getting-started-with-linux/lab-01-bootstrap-and-baseline-linux-server.md
```

### Canonical Placement Rules

| Lab | Folder | Chapter |
| --- | --- | --- |
| 01 | `01-getting-started-with-linux/` | Getting Started with Linux |
| 02 | `02-working-with-permissions-and-privileged-accounts/` | Working with Permissions and Privileged Accounts |
| 03 | `03-customizing-the-user-experience/` | Customizing the User Experience |
| 04 | `04-managing-users/` | Managing Users |
| 05 | `05-connecting-to-a-network/` | Connecting to a Network |
| 06 | `06-installing-and-uninstalling-software/` | Installing and Uninstalling Software |
| 07 | `07-managing-storage/` | Managing Storage |
| 08 | `08-maintaining-system-health/` | Maintaining System Health |
| 09 | `09-monitoring-your-system/` | Monitoring Your System |
| 10 | `10-scripting-and-automation/` | Scripting and Automation |
| 11 | `11-deploying-samba-for-windows-compatibility/` | Deploying Samba for Windows Compatibility |
| 12 | `12-troubleshooting-linux/` | Troubleshooting Linux |
| 13 | `13-securing-your-system/` | Securing Your System |
| 14 | `14-continuing-your-education/` | Continuing Your Education |
| 15 | `15-making-career-moves/` | Making Career Moves |

### Cross-Cutting Topics

Some topics appear across multiple labs rather than as standalone folders:

* AI-assisted operations
* RHEL vs Ubuntu comparison
* operational documentation
* troubleshooting discipline
* post-reboot verification
* security and privacy review
* production readiness

### Upload Rule

Final lab write-ups must be uploaded to the matching chapter folder.

Labs should not be uploaded to the repository root.
