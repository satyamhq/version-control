# Git HEAD – Complete Notes

## Overview
Every Git repository contains a hidden folder called `.git`.  
This folder stores **all metadata** required by Git to track changes, commits, and branches.

One of the most important files inside `.git` is called **HEAD**.

---

## What is HEAD?
- `HEAD` is a **special pointer**
- It tells Git:
  - Which **branch** you are currently on
  - Which **commit** you are currently viewing

In short:
> **HEAD always points to the latest commit of the current branch**

---

## Locating the HEAD File

Move into the `.git` directory:
```bash
cd .git
