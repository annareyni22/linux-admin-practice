# Memory Management

## Check Memory Usage

```bash
free -m
```

## Display Memory in Human Readable Format

```bash
free -h
```

## Virtual Memory Statistics

```bash
vmstat
```

## Top Memory Consumers

```bash
ps aux --sort=-%mem
```

## Production Troubleshooting Example

Issue:
Server running slowly.

Steps:

```bash
free -h
```

Check available memory.

```bash
vmstat 1 5
```

Monitor memory pressure.

```bash
top
```

Look for processes consuming excessive memory.
