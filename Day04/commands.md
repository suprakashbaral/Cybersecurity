# Day 04 Commands

## View Permissions

```bash
ls -l
```

---

## View Hidden Files with Permissions

```bash
ls -la
```

---

## Change Permissions

```bash
chmod 755 script.sh
```

---

## Add Execute Permission

```bash
chmod +x script.sh
```

---

## Remove Write Permission

```bash
chmod -w report.txt
```

---

## Change Owner

```bash
sudo chown user:user report.txt
```

---

## Change Group

```bash
sudo chgrp developers report.txt
```

---

## View Current umask

```bash
umask
```

---

## Change umask

```bash
umask 022
```

---

## Find SUID Files

```bash
find / -perm -4000 2>/dev/null
```

---

## Find SGID Files

```bash
find / -perm -2000 2>/dev/null
```