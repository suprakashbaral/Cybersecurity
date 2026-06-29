# Day 05 Commands

## View Running Processes

```bash
ps
```

---

## Detailed Process List

```bash
ps -ef
```

---

## User-Friendly Process List

```bash
ps aux
```

---

## Real-Time Process Monitor

```bash
top
```

---

## Improved Process Viewer

```bash
htop
```

Install:

```bash
sudo apt install htop
```

---

## Search Processes

```bash
pgrep firefox
```

---

## Search Using grep

```bash
ps aux | grep ssh
```

---

## Kill Process

```bash
kill PID
```

---

## Force Kill

```bash
kill -9 PID
```

---

## Kill by Name

```bash
pkill firefox
```

---

## Process Tree

```bash
pstree
```

Install:

```bash
sudo apt install psmisc
```

---

## Background Job

```bash
sleep 100 &
```

---

## Display Background Jobs

```bash
jobs
```

---

## Bring Job to Foreground

```bash
fg
```

---

## Change Priority

```bash
nice -n 10 command
```

---

## Modify Running Process Priority

```bash
renice 5 PID
```