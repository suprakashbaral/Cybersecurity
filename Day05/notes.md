# Day 05 - Linux Process Management & Monitoring

# Introduction

A process is a running instance of a program. Every application, service, or command executed in Linux creates one or more processes.

Examples:

- Firefox
- Google Chrome
- SSH Server
- Apache
- Python Script
- Bash Terminal

Cybersecurity professionals constantly monitor processes to detect suspicious activity such as malware, reverse shells, ransomware, unauthorized miners, or compromised services.

---

# What is a Process?

A process is a program currently executing in memory.

Each process has:

- Process ID (PID)
- Parent Process ID (PPID)
- User Owner
- CPU Usage
- Memory Usage
- Start Time
- Current State

---

# Process States

Running (R)

The process is currently executing.

Sleeping (S)

Waiting for an event.

Stopped (T)

Temporarily paused.

Zombie (Z)

Finished execution but still waiting for the parent process to collect its exit status.

---

# Parent and Child Processes

Every process starts from another process.

Example:

systemd (PID 1)
 └── bash
      └── python
           └── script.py

Understanding parent-child relationships helps identify suspicious activity.

---

# Why Process Monitoring is Important?

Process monitoring helps detect:

- Malware
- Reverse Shells
- Cryptocurrency Miners
- Privilege Escalation
- Persistence Mechanisms
- Unauthorized Programs
- High CPU Usage
- Memory Abuse

---

# Important Process Information

PID

Unique identifier.

PPID

Parent Process ID.

UID

User running the process.

TTY

Terminal associated with the process.

CPU %

Processor usage.

MEM %

Memory usage.

---

# Signals

Linux communicates with processes using signals.

Common Signals

SIGTERM (15)

Gracefully terminate a process.

SIGKILL (9)

Forcefully kill a process.

SIGSTOP (19)

Pause a process.

SIGCONT (18)

Resume a paused process.

---

# Nice Value

Controls process priority.

Range:

-20 (Highest Priority)

19 (Lowest Priority)

Lower nice values receive more CPU time.

---

# Cybersecurity Perspective

Attackers often:

- Hide malicious processes.
- Rename malware to appear legitimate.
- Spawn reverse shells.
- Create persistence using background processes.

SOC analysts regularly investigate unusual process trees, high resource usage, and unauthorized services.

---

# Summary

Today I learned how Linux manages processes, how to identify process information, understand process states, signals, priorities, and why process monitoring is essential for detecting cyber threats.