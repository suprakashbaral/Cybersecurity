# Day 04 - Linux File Permissions & Privilege Escalation Basics

# Introduction

Linux protects files and directories using a permission system. These permissions determine who can read, write, or execute files.

A strong understanding of file permissions is essential because many Linux security incidents occur due to incorrect permissions or privilege misconfigurations.

---

# Why Learn File Permissions?

File permissions help to:

- Protect sensitive files.
- Prevent unauthorized access.
- Restrict modifications.
- Secure executable programs.
- Reduce the risk of privilege escalation.

Cybersecurity professionals regularly inspect permissions during security audits and incident investigations.

---

# Permission Categories

Every file has three permission categories.

1. Owner (u)
2. Group (g)
3. Others (o)

Example:

-rwxr-x---

Owner : rwx
Group : r-x
Others: ---

---

# Permission Types

## Read (r)

Value: 4

Allows viewing the file contents.

Example:

cat report.txt

---

## Write (w)

Value: 2

Allows modifying the file.

Examples:

nano report.txt

echo "Hello" >> report.txt

---

## Execute (x)

Value: 1

Allows running a program or script.

Example:

./script.sh

---

# Understanding Permission Output

Example:

-rwxr-xr--

Breakdown:

-

Regular file

rwx

Owner has Read, Write, Execute

r-x

Group has Read and Execute

r--

Others have Read only

---

# Numeric Permissions

Permission values

Read = 4

Write = 2

Execute = 1

Examples

777 = rwxrwxrwx

755 = rwxr-xr-x

750 = rwxr-x---

700 = rwx------

644 = rw-r--r--

600 = rw-------

400 = r--------

---

# chmod

The chmod command changes file permissions.

Example:

chmod 755 script.sh

Grant execute permission:

chmod +x script.sh

Remove write permission:

chmod -w file.txt

---

# chown

Changes file ownership.

Example:

sudo chown user:user report.txt

---

# chgrp

Changes group ownership.

Example:

sudo chgrp developers report.txt

---

# umask

Defines the default permissions for newly created files.

Display current umask:

umask

Example:

umask 022

---

# Special Permissions

Linux supports three special permission bits.

## SUID (Set User ID)

Runs a program with the owner's privileges.

Example:

passwd

Permission:

-rwsr-xr-x

Security Risk:

Attackers may exploit vulnerable SUID binaries to gain elevated privileges.

---

## SGID (Set Group ID)

Files execute with the group's permissions.

Directories inherit the group.

Useful for shared project folders.

---

## Sticky Bit

Applied mainly to shared directories.

Only the file owner or root can delete files.

Example:

/tmp

Permission:

drwxrwxrwt

---

# Principle of Least Privilege

Always assign the minimum permissions required.

Avoid:

777

Preferred:

644 for files

755 for executable scripts

700 for sensitive directories

---

# Cybersecurity Perspective

Incorrect permissions can lead to:

- Unauthorized data access
- Privilege escalation
- Malware execution
- Credential theft
- Insider attacks

Security analysts regularly audit permissions to detect weaknesses.

---

# Summary

Today I learned how Linux controls file access using permissions. I also explored chmod, chown, chgrp, umask, SUID, SGID, and Sticky Bit, and understood how permission misconfigurations can create security vulnerabilities.