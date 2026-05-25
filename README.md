# Multi-OS Administration & Security Audit

A comprehensive security audit focusing on the deployment and management of a secure multi-user Linux environment. This project demonstrates core system administration skills including user provisioning, access control, and network diagnostics.

## What It Does

This audit establishes a secure corporate Linux infrastructure by:

- Creating structured directory hierarchies for organizational data
- Provisioning user accounts and security groups
- Implementing the Principle of Least Privilege (PoLP)
- Verifying network integrity using diagnostic tools

## Security Measures Implemented

### 1. Directory Architecture

```bash
mkdir -p ~/Portfolio/Operating_System_Becoming_a_Power_User
```

- Organized multi-tier file system for portfolio management

### 2. Identity Management

```bash
addgroup finance_dept
adduser stanley_admin
```

- Provisioned security group (finance_dept)
- Created administrative user (stanley_admin)
- Assigned encrypted passwords for local authentication

### 3. Access Control (Principle of Least Privilege)

```bash
chown :finance_dept /home/stanley_admin/salary_details.txt
chmod 640 /home/stanley_admin/salary_details.txt
```

- **Owner**: Read/Write access (6)
- **Group**: Read-only access (4)
- **Others**: No access (0)

## Core Competencies Demonstrated

| Skill | Tools Used | Outcome |
|-------|-----------|---------|
| Identity Management | addgroup, adduser | Secure administrative roles |
| Access Control | chmod, chown | Applied PoLP |
| Infrastructure Analysis | ping, traceroute, nslookup | Verified network integrity |
| File System Management | mkdir, pwd, ls | Organized data structure |

## Troubleshooting Notes

During the audit, certain kernel-level network commands (ip addr, ifconfig) were restricted due to the emulated ISH environment. To ensure completion, I utilized host-level diagnostics, demonstrating adaptability in constrained virtualized environments.

## What I Learned

- Linux user and group management
- File permission bit-masks (chmod, chown)
- The Principle of Least Privilege in practice
- Network diagnostics in restricted environments
- Problem-solving when standard tools are unavailable

## Environment

- Platform: Linux (Alpine/ISH Environment)
- Shell: Bash
- Date: March 2026
