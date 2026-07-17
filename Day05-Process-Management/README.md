# Day 05 - Process Management

## Objective

Learn how Linux processes work, how to monitor them, and how to manage or terminate them when required.

---

# What is a Process?

A process is a program that is currently running in the system.

Examples:

- Chrome Browser
- VS Code
- Jenkins
- Docker
- Nginx

All running applications are treated as processes by Linux.

---

# Why is Process Management Important in DevOps?

As a DevOps Engineer, you will frequently:

- Check whether an application is running
- Monitor CPU and memory usage
- Identify stuck processes
- Restart failed applications
- Troubleshoot production servers

Understanding process management is essential for maintaining system health.

---

# 1. ps Command

## Purpose

Used to display currently running processes.

## Syntax

```bash
ps
```

## Example

```bash
ps
```

## Advanced Usage

```bash
ps -ef
```

### What does ps -ef show?

- User
- PID (Process ID)
- Start Time
- Running Command

### Use Case

Check whether an application is running.

### Example

```bash
ps -ef | grep nginx
```

### Interview Question

Q: How do you check running processes in Linux?

Answer:

```bash
ps -ef
```

---

# 2. top Command

## Purpose

Used to monitor processes in real time.

## Syntax

```bash
top
```

## Information Displayed

- CPU Usage
- Memory Usage
- Running Processes
- System Load

### Use Case

Application is slow and users are reporting performance issues.

Use:

```bash
top
```

to identify high CPU or memory consuming processes.

### Interview Question

Q: Which command is used to monitor CPU and Memory usage?

Answer:

```bash
top
```

---

# 3. htop Command

## Purpose

Advanced and interactive version of top.

## Syntax

```bash
htop
```

## Benefits

- Easier to read
- Interactive interface
- Better process monitoring

### Installation

```bash
sudo apt install htop
```

### Use Case

Monitor resource utilization in an easier format.

---

# 4. PID (Process ID)

## What is PID?

PID stands for Process ID.

Every running process gets a unique number.

### Example

```text
PID = 1234
PID = 5678
```

### Why is PID Important?

Linux uses PID to identify and manage processes.

### Interview Question

Q: What is PID?

Answer:

A unique identifier assigned to each running process.

---

# 5. kill Command

## Purpose

Used to stop a running process.

## Syntax

```bash
kill PID
```

## Example

```bash
kill 1234
```

### Use Case

Terminate a misbehaving application.

### Interview Question

Q: How do you stop a running process?

Answer:

```bash
kill PID
```

---

# 6. kill -9 Command

## Purpose

Forcefully terminates a process.

## Syntax

```bash
kill -9 PID
```

## Example

```bash
kill -9 1234
```

### When to Use?

When a normal kill command does not stop the process.

### Interview Question

Q: Difference between kill and kill -9?

Answer:

kill:
- Graceful termination

kill -9:
- Forceful termination

---

# 7. pkill Command

## Purpose

Terminates processes by name.

## Syntax

```bash
pkill process_name
```

## Example

```bash
pkill nginx
```

### Use Case

Kill a process without finding its PID.

### Interview Question

Q: How do you kill a process without knowing its PID?

Answer:

```bash
pkill process_name
```

---

# 8. Background Process (&)

## Purpose

Runs a process in the background.

## Example

```bash
sleep 100 &
```

### Why Use Background Processes?

Allows the terminal to remain free while the task continues executing.

---

# 9. jobs Command

## Purpose

Displays background jobs running in current terminal.

## Example

```bash
jobs
```

### Use Case

Check whether background tasks are running.

---

# 10. fg Command

## Purpose

Brings a background process to the foreground.

## Example

```bash
fg
```

### Use Case

Need to interact with a background process again.

---

# 11. bg Command

## Purpose

Moves a stopped process to the background.

## Example

```bash
bg
```

### Use Case

Continue executing a process in the background.

---

# Real DevOps Scenarios

## Scenario 1: Application Not Running

Check:

```bash
ps -ef | grep application_name
```

Verify whether the application process exists.

---

## Scenario 2: High CPU Usage

Check:

```bash
top
```

Identify the process consuming CPU.

Stop it if required.

```bash
kill PID
```

---

## Scenario 3: Process Stuck or Hanging

Forcefully terminate:

```bash
kill -9 PID
```

---

## Scenario 4: Stop All Nginx Processes

```bash
pkill nginx
```

---

# Hands-On Practice

Run the following commands:

```bash
ps

ps -ef

top

sleep 100 &

jobs

fg

bg
```

Check a specific process:

```bash
ps -ef | grep bash
```

---

# Interview Questions

## What is a process?

A process is a running instance of a program.

---

## What is PID?

PID stands for Process ID and uniquely identifies a running process.

---

## How do you view running processes?

```bash
ps -ef
```

---

## How do you monitor CPU and Memory utilization?

```bash
top
```

---

## Difference between kill and kill -9?

kill:
- Graceful termination

kill -9:
- Forceful termination

---

## How do you terminate a process by name?

```bash
pkill process_name
```

---

## What is a background process?

A process that runs without occupying the current terminal session.

---

## What do fg and bg do?

fg:
- Brings process to foreground

bg:
- Moves process to background

---

# Day 05 Summary

Topics Covered:

✅ Process

✅ PID

✅ ps

✅ ps -ef

✅ top

✅ htop

✅ kill

✅ kill -9

✅ pkill

✅ jobs

✅ fg

✅ bg

Day 05 Status: Completed ✅
