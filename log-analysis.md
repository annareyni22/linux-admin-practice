# Log Analysis

## View File Contents

```bash
cat logfile.log
```

## Read Large Files

```bash
less logfile.log
```

## View Last Lines

```bash
tail logfile.log
```

## Follow Logs in Real Time

```bash
tail -f logfile.log
```

## Search for Errors

```bash
grep ERROR logfile.log
```

## Count Error Occurrences

```bash
grep ERROR logfile.log | wc -l
```

## System Logs

```bash
journalctl
```

## Service Logs

```bash
journalctl -u nginx
```

## Production Troubleshooting Example

Issue:
Application returning HTTP 500.

Steps:

1. Check application logs

```bash
tail -f application.log
```

2. Search for errors

```bash
grep ERROR application.log
```

3. Check service logs

```bash
journalctl -u service-name
```

4. Identify root cause and correlate timestamps.
