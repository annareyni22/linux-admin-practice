# Process Management

## View Running Processes

```bash
ps aux
```

Displays all running processes.

## Interactive Process Viewer

```bash
top
```

Shows CPU and memory utilization in real time.

## Enhanced Process Viewer

```bash
htop
```

User-friendly process monitoring tool.

## Find Process by Name

```bash
ps -ef | grep nginx
```

## Kill Process

```bash
kill <PID>
```

Example:

```bash
kill 1234
```

## Force Kill

```bash
kill -9 <PID>
```

## Production Troubleshooting Example

Problem:
Application is slow.

Investigation:

```bash
top
```

Check CPU utilization.

```bash
ps aux --sort=-%cpu
```

Identify high CPU-consuming processes.

```bash
ps aux --sort=-%mem
```

Identify memory-heavy processes.
