# Day 03 - Users, Groups & Privileges

# Introduction

Linux is a multi-user operating system. Multiple users can access the same computer while keeping their files and permissions separate.

Managing users and permissions is one of the most important responsibilities of a Linux administrator and cybersecurity professional.

---

# Why Learn Users and Permissions?

Attackers often try to:

- Steal user credentials.
- Escalate privileges.
- Create unauthorized users.
- Modify permissions.
- Access restricted files.

Defenders monitor user accounts and enforce proper permissions to protect systems.

---

# Types of Users

## Root User

The root user is the administrator of Linux.

Characteristics:

- User ID (UID): 0
- Has unrestricted access.
- Can modify any file.
- Can install or remove software.
- Can manage all users.

Example:

```bash
sudo su
```

⚠️ Use root privileges carefully because incorrect commands can damage the system.

---

## Regular User

A regular user has limited permissions.

Example:

suprakash

Regular users cannot modify system files without permission.

---

## System Users

System users are created automatically for services.

Examples:

www-data

mysql

postgres

These accounts usually cannot log in interactively.

---

# User ID (UID)

Each Linux user has a unique numeric identifier.

Example:

Root

UID = 0

Normal users

UID = 1000+

Display current UID:

```bash
id
```

---

# Groups

Groups allow multiple users to share permissions.

Example:

sudo

docker

adm

Users can belong to multiple groups.

Display groups:

```bash
groups
```

---

# Principle of Least Privilege

Users should receive only the permissions they need to perform their work.

Benefits:

- Limits damage if an account is compromised.
- Reduces insider threats.
- Improves security.

---

# Sudo

The sudo command allows a regular user to execute commands with administrator privileges.

Example:

```bash
sudo apt update
```

Only trusted users should be members of the sudo group.

---

# Important Files

## /etc/passwd

Contains user account information.

Example entry:

```
student:x:1000:1000:Student:/home/student:/bin/bash
```

---

## /etc/shadow

Stores encrypted password hashes.

Only root can read this file.

---

## /etc/group

Contains group information.

---

# Why This Matters in Cybersecurity

Cybersecurity professionals investigate:

- Unauthorized accounts
- Privilege escalation
- Password attacks
- Misconfigured permissions
- Compromised service accounts
- Insider threats

Understanding Linux users and permissions is essential for penetration testing, digital forensics, and incident response.

---

# Summary

Today I learned how Linux manages users, groups, and privileges. I also explored important system files like `/etc/passwd`, `/etc/shadow`, and `/etc/group`, and understood why proper privilege management is a critical security practice.