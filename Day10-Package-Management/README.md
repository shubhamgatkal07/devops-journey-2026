# Day 10 - Package Management

## Objective

Learn how software is installed, updated and managed in Linux.

---

# What is a Package?

A package is a software bundle containing application files, dependencies and configuration files.

Examples:

- Docker
- Jenkins
- Nginx

---

# What is Package Management?

Package management helps:

- Install software
- Upgrade software
- Remove software
- Manage dependencies

---

# Package Managers

Ubuntu/Debian:

```bash
apt
```

RHEL/CentOS:

```bash
yum
```

or

```bash
dnf
```

---

# apt

## Update Package Repository

```bash
sudo apt update
```

## Upgrade Packages

```bash
sudo apt upgrade
```

## Install Package

```bash
sudo apt install nginx
```

## Remove Package

```bash
sudo apt remove nginx
```

---

# yum

## Install Package

```bash
sudo yum install nginx
```

## Update Packages

```bash
sudo yum update
```

---

# dnf

## Install Package

```bash
sudo dnf install nginx
```

## Update Packages

```bash
sudo dnf update
```

---

# dpkg

## Install .deb Package

```bash
sudo dpkg -i package.deb
```

## List Installed Packages

```bash
dpkg -l
```

---

# rpm

## Install RPM Package

```bash
rpm -ivh package.rpm
```

## List Installed RPM Packages

```bash
rpm -qa
```

---

# Real DevOps Scenarios

1. Install Docker
2. Install Jenkins
3. Update Server Packages
4. Manage Software Dependencies

---

# Interview Questions

## What is a package?

A software bundle containing application files, dependencies and configuration.

---

## What is apt?

Package manager used in Ubuntu and Debian systems.

---

## Difference between apt update and apt upgrade?

update:
Refresh package list

upgrade:
Install newer versions

---

## What is yum?

Package manager for RedHat-based distributions.

---

## What is dnf?

A newer version of yum.

---

## What is dpkg?

Used to manage .deb packages.

---

## What is rpm?

Used to manage .rpm packages.
