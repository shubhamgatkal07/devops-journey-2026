# Day 04 - Users and Groups

## Objective

Learn how Linux users, groups, and administrative privileges work.

---

## Topics Learned

- User
- Group
- Root User
- sudo
- whoami
- id
- groups
- useradd
- groupadd
- usermod
- passwd

---

## User

A user is an account that can access a Linux system.

Examples:

- shubham
- root
- ubuntu
- jenkins

---

## Group

A group is a collection of users.

Groups make permission management easier.

Example:

DevOps Team

- User1
- User2
- User3

---

## Root User

The root user is the superuser in Linux.

Root has full access to:

- Files
- Users
- Services
- Applications

---

## sudo

sudo stands for:

Super User Do

It allows a normal user to execute commands with administrative privileges.

Example:

sudo systemctl restart nginx

---

# Commands Learned

## whoami

Purpose:

Displays current logged-in user.

Example:

whoami

---

## id

Purpose:

Displays user ID, group ID and group information.

Example:

id

---

## groups

Purpose:

Displays all groups of the current user.

Example:

groups

---

## useradd

Purpose:

Creates a new user.

Example:

sudo useradd devops

---

## passwd

Purpose:

Sets or changes a user password.

Example:

sudo passwd devops

---

## groupadd

Purpose:

Creates a new group.

Example:

sudo groupadd devops

---

## usermod

Purpose:

Modifies an existing user.

Example:

sudo usermod -aG devops shubham

---

# Hands-On Practice

Commands Executed:

whoami

id

groups

sudo useradd testuser

sudo groupadd devops

sudo usermod -aG devops testuser

sudo passwd testuser

---

# Real DevOps Scenario

A new developer joins the company.

Steps:

1. Create a user account.
2. Create a group.
3. Add the user to the group.
4. Provide required permissions.
5. Verify access.

Commands:

sudo useradd developer1

sudo groupadd devops

sudo usermod -aG devops developer1

sudo passwd developer1

---

# Interview Questions

## What is a user?

A user is an account used to access a Linux system.

---

## What is a group?

A group is a collection of users used for permission management.

---

## What is root user?

Root is the superuser with full administrative privileges.

---

## What is sudo?

sudo allows a normal user to run commands with administrative privileges.

---

## Difference between user and group?

User = Individual account

Group = Collection of users

---

## How do you create a user?

sudo useradd username

Example:

sudo useradd devops

---

## How do you create a group?

sudo groupadd groupname

Example:

sudo groupadd devops

---

## How do you add a user to a group?

sudo usermod -aG groupname username

Example:

sudo usermod -aG devops shubham

---

## What does whoami do?

Displays current logged-in user.

---

## What does id do?

Displays user ID, group ID, and group membership.
