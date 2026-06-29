# Day 05 Practice

## Task 1

View all running processes.

```bash
ps aux
```

---

## Task 2

Open top.

```bash
top
```

Press q to quit.

---

## Task 3

Install htop.

```bash
sudo apt install htop
```

---

## Task 4

Run htop.

```bash
htop
```

---

## Task 5

Display process tree.

```bash
pstree
```

---

## Task 6

Create a background process.

```bash
sleep 300 &
```

---

## Task 7

Display jobs.

```bash
jobs
```

---

## Task 8

Find the PID of the sleep process.

```bash
pgrep sleep
```

---

## Task 9

Terminate it gracefully.

```bash
kill PID
```

---

## Task 10

Run another sleep process and terminate it with SIGKILL.

```bash
sleep 500 &
kill -9 PID
```