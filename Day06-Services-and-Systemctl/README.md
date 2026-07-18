# Day 06 - Services and Systemctl

## Objective

Learn how to manage Linux services using the systemctl command.

---

# What is a Service?

A service is a program that runs in the background and continuously provides functionality to the system.

Examples:

- nginx
- docker
- jenkins
- ssh
- mysql

---

# What is systemctl?

systemctl is a Linux command used to manage services.

Using systemctl we can:

- Start services
- Stop services
- Restart services
- Check service status
- Enable services during boot

---

# Commands Learned

## Check Service Status

```bash
systemctl status nginx
```

Purpose:

Check whether a service is running, stopped, or failed.

---

## Start Service

```bash
sudo systemctl start nginx
```

Purpose:

Starts a stopped service.

---

## Stop Service

```bash
sudo systemctl stop nginx
```

Purpose:

Stops a running service.

---

## Restart Service

```bash
sudo systemctl restart nginx
```

Purpose:

Stops and starts the service again.

---

## Reload Service

```bash
sudo systemctl reload nginx
```

Purpose:

Reloads configuration without restarting the service.

---

## Enable Service

```bash
sudo systemctl enable nginx
```

Purpose:

Starts the service automatically after system reboot.

---

## Disable Service

```bash
sudo systemctl disable nginx
```

Purpose:

Prevents the service from starting automatically after reboot.

---

## List Running Services

```bash
systemctl list-units --type=service
```

Purpose:

Displays currently running services.

---

## Check Failed Services

```bash
systemctl --failed
```

Purpose:

Displays failed services.

---

# Real DevOps Scenarios

## Scenario 1: Website is Down

Check nginx status:

```bash
systemctl status nginx
```

If stopped:

```bash
sudo systemctl start nginx
```

---

## Scenario 2: Docker Commands Not Working

Check:

```bash
systemctl status docker
```

Restart:

```bash
sudo systemctl restart docker
```

---

## Scenario 3: Jenkins Dashboard Not Opening

Check:

```bash
systemctl status jenkins
```

If service is down:

```bash
sudo systemctl start jenkins
```

---

# Interview Questions and Answers

## What is a service?

A service is a background application that continuously runs and provides functionality to the system.

Examples:

- Docker
- Jenkins
- Nginx
- SSH

---

## What is systemctl?

systemctl is a command used to manage Linux services.

---

## How do you check service status?

```bash
systemctl status service_name
```

Example:

```bash
systemctl status nginx
```

---

## How do you start a service?

```bash
sudo systemctl start service_name
```

---

## How do you stop a service?

```bash
sudo systemctl stop service_name
```

---

## How do you restart a service?

```bash
sudo systemctl restart service_name
```

---

## Difference between restart and reload?

Restart:

- Stops service
- Starts service again

Reload:

- Applies configuration changes
- Service continues running

---

## How do you enable a service at boot time?

```bash
sudo systemctl enable service_name
```

---

## How do you disable a service from starting automatically?

```bash
sudo systemctl disable service_name
```

---

## How do you check failed services?

```bash
systemctl --failed
```


