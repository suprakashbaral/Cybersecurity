# Day 04 Practice

## Task 1

Create a file.

```bash
touch secret.txt
```

---

## Task 2

View permissions.

```bash
ls -l
```

---

## Task 3

Give execute permission.

```bash
chmod +x secret.txt
```

---

## Task 4

Change permission to 600.

```bash
chmod 600 secret.txt
```

---

## Task 5

Create a script.

```bash
nano hello.sh
```

Contents:

```bash
#!/bin/bash
echo "Hello Cybersecurity"
```

---

## Task 6

Make it executable.

```bash
chmod +x hello.sh
```

---

## Task 7

Run it.

```bash
./hello.sh
```

---

## Task 8

Display current umask.

```bash
umask
```

---

## Task 9

Find all SUID files.

```bash
find / -perm -4000 2>/dev/null
```

---

## Task 10

Find all SGID files.

```bash
find / -perm -2000 2>/dev/null
```