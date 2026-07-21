# Day 09 - SSH, SCP and Remote Server Access

## Objective

Learn how DevOps Engineers securely access remote servers and transfer files between systems.

---

# What is SSH?

SSH stands for Secure Shell.

It is a secure protocol used to connect to and manage remote Linux servers.

Example:

Laptop
↓
SSH
↓
Linux Server

---

# Why is SSH Important in DevOps?

DevOps Engineers use SSH to:

- Access cloud servers
- Check logs
- Restart services
- Deploy applications
- Troubleshoot production issues

---

# SSH Command

## Syntax

```bash
ssh username@ip-address
```

## Example

```bash
ssh ubuntu@192.168.1.10
```

---

# SSH Using Private Key

## Syntax

```bash
ssh -i key.pem username@ip-address
```

## Example

```bash
ssh -i mykey.pem ubuntu@54.12.34.56
```

---

# Why Use SSH Keys?

Benefits:

- More secure than passwords
- Faster authentication
- Common in AWS, Azure, and GCP

---

# What is SCP?

SCP stands for Secure Copy.

It is used to transfer files securely between local and remote systems.

---

# Copy File to Remote Server

## Syntax

```bash
scp file.txt user@server:/path
```

## Example

```bash
scp app.zip ubuntu@54.12.34.56:/home/ubuntu
```

---

# Copy File from Remote Server

## Syntax

```bash
scp user@server:/path/file.txt .
```

## Example

```bash
scp ubuntu@54.12.34.56:/home/ubuntu/log.txt .
```

---

# Important SSH Files

## .ssh Directory

Location:

```bash
~/.ssh
```

Contains:

- SSH Keys
- Known Hosts
- Authorized Keys

---

# authorized_keys

Location:

```bash
~/.ssh/authorized_keys
```

Purpose:

Stores public keys that are allowed to access the server.

---

# known_hosts

Location:

```bash
~/.ssh/known_hosts
```

Purpose:

Stores information about previously connected servers.

---

# Generate SSH Key

Command:

```bash
ssh-keygen
```

Purpose:

Generates public and private SSH keys.

---

# View Public Key

Command:

```bash
cat ~/.ssh/id_rsa.pub
```

Purpose:

Displays the public key which can be added to a remote server.

---

# Real DevOps Scenarios

## Scenario 1: Access AWS EC2 Server

```bash
ssh -i mykey.pem ubuntu@server-ip
```

---

## Scenario 2: Upload Application Build

```bash
scp app.jar ubuntu@server-ip:/opt/application
```

---

## Scenario 3: Download Server Logs

```bash
scp ubuntu@server-ip:/var/log/app.log .
```

---

## Scenario 4: Troubleshoot Website Issue

```bash
ssh ubuntu@server-ip

systemctl status nginx
```

---

# Hands-On Practice

Commands Practiced:

```bash
ssh localhost

ssh-keygen

cat ~/.ssh/id_rsa.pub
```

---

# Interview Questions and Answers

## What is SSH?

SSH (Secure Shell) is a secure protocol used for remote login and server management.

---

## Why is SSH used in DevOps?

SSH allows DevOps Engineers to securely access and manage remote Linux servers.

---

## What is the default SSH port?

Port 22

---

## How do you connect to a remote server?

```bash
ssh username@ip-address
```

---

## How do you connect using a private key?

```bash
ssh -i key.pem username@ip-address
```

---

## What is SCP?

SCP is a secure file transfer utility that uses SSH protocol.

---

## How do you upload a file to a server?

```bash
scp file.txt user@server:/path
```

---

## How do you download a file from a server?

```bash
scp user@server:/path/file.txt .
```

---

## What is authorized_keys?

A file that stores public keys allowed to access the server.

---

## What is known_hosts?

A file that stores information about previously connected servers.

---

# Day 09 Summary


