# Day 08 - Linux Networking Fundamentals

## Objective

Learn basic networking commands used in Linux and DevOps.

---

# What is an IP Address?

An IP address is a unique address used to identify a device on a network.

---

# Commands Learned

## ping

Purpose:
Check connectivity between systems.

Example:

```bash
ping google.com
```

---

## curl

Purpose:
Send HTTP requests and test APIs.

Example:

```bash
curl https://google.com
```

---

## wget

Purpose:
Download files from internet.

Example:

```bash
wget https://example.com/file.zip
```

---

## netstat

Purpose:
Check open ports and active connections.

Example:

```bash
netstat -tuln
```

---

## ss

Purpose:
Display listening ports and active connections.

Example:

```bash
ss -tuln
```

---

## nslookup

Purpose:
Check DNS resolution.

Example:

```bash
nslookup google.com
```

---

## dig

Purpose:
Perform detailed DNS lookup.

Example:

```bash
dig google.com
```

---

# Real DevOps Scenarios

1. Website Not Reachable
2. DNS Issues
3. API Testing
4. Port Verification

---

# Interview Questions

## What is an IP Address?

A unique address assigned to a device on a network.

---

## What does ping do?

Checks network connectivity.

---

## What is curl used for?

Testing APIs and websites.

---

## Difference between curl and wget?

curl = Send requests

wget = Download files

---

## How do you check open ports?

```bash
ss -tuln
```

or

```bash
netstat -tuln
```

---

## What does nslookup do?

Checks DNS resolution.

---

## Difference between nslookup and dig?

nslookup = Basic DNS query

dig = Detailed DNS troubleshooting.
