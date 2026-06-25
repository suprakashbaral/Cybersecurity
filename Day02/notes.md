# Day 02 Notes

# Linux File System

The Linux file system is a hierarchical structure that organizes all files and directories starting from a single root directory (/). Everything in Linux, including files, folders, devices, and processes, is represented as part of this file system.

Unlike Windows, Linux does not use drive letters such as C: or D:. Instead, all storage devices are mounted under the root directory.

---

# What is a Directory?

A directory is a folder that stores files and other directories.

Example:

/
├── home
├── etc
├── var
├── usr

Directories help organize the operating system and user files.

---

# Root Directory (/)

The root directory is the top-most directory in Linux.

Every file and directory starts from the root directory.

Example:

/

Everything inside Linux is accessed through the root directory.

---

# Important Linux Directories

## /home

Stores personal files of users.

Example:

/home/suprakash

---

## /root

Home directory of the root (administrator) user.

---

## /bin

Contains essential user commands.

Examples:

- ls
- cp
- mv
- cat

---

## /etc

Stores system configuration files.

Examples:

- passwd
- hosts
- network configuration

---

## /usr

Contains installed software, libraries, and documentation.

---

## /var

Stores variable data such as logs, cache, mail, and temporary files.

---

## /tmp

Stores temporary files.

These files may be deleted automatically when the system restarts.

---

## /dev

Contains device files.

Examples:

- Hard disks
- USB devices
- Keyboard
- Mouse

---

## /boot

Contains files required for booting Linux.

---

## /proc

A virtual directory that provides information about running processes and the Linux kernel.

---

# Why is the Linux File System Important?

Understanding the Linux file system helps cybersecurity professionals:

- Locate log files.
- Investigate security incidents.
- Analyze malware.
- Perform digital forensic investigations.
- Configure servers.
- Manage users and permissions.

---

# Summary

Today I learned how Linux organizes files using a hierarchical directory structure. I also learned the purpose of important system directories and why understanding them is essential for cybersecurity and system administration.

---

Date: 26 June 2026