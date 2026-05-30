# Networking Commands

## Check IP Address

```bash
ip addr
```

or

```bash
ifconfig
```

## Check Routing Table

```bash
ip route
```

## Test Connectivity

```bash
ping google.com
```

## DNS Lookup

```bash
nslookup google.com
```

```bash
dig google.com
```

## Check Open Ports

```bash
ss -tulpn
```

## Check Listening Services

```bash
netstat -tulpn
```

## Test HTTP Connectivity

```bash
curl -v https://example.com
```

## Production Troubleshooting Example

Issue:
Application is unreachable.

Steps:

1. Verify server is reachable

```bash
ping <host>
```

2. Verify DNS resolution

```bash
nslookup <hostname>
```

3. Verify application port

```bash
ss -tulpn
```

4. Verify application endpoint

```bash
curl -v http://application-url
```
