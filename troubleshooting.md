# Linux Troubleshooting Scenarios

## Scenario 1: High CPU Usage

### Investigation

```bash
top
```

```bash
ps aux --sort=-%cpu
```

### Actions

* Identify process consuming CPU
* Check logs
* Verify recent changes
* Restart service if required

---

## Scenario 2: High Memory Usage

### Investigation

```bash
free -h
```

```bash
ps aux --sort=-%mem
```

### Actions

* Identify memory-heavy processes
* Check for memory leaks
* Review application logs

---

## Scenario 3: Disk Full

### Investigation

```bash
df -h
```

```bash
du -sh /*
```

### Actions

* Locate large files
* Archive or remove old logs
* Verify disk growth patterns

---

## Scenario 4: Service Not Running

### Investigation

```bash
systemctl status service-name
```

### Actions

```bash
systemctl restart service-name
```

Review logs:

```bash
journalctl -u service-name
```

---

## Scenario 5: Application Not Reachable

### Investigation

```bash
ping hostname
```

```bash
nslookup hostname
```

```bash
curl -v application-url
```

### Actions

* Verify service status
* Verify network connectivity
* Verify firewall rules
* Check application logs
