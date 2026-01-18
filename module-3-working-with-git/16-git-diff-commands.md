# Git Diff Commands

## Introduction
Great novels are rarely written in one go. Authors usually go through many drafts before reaching the final version. Sometimes, an idea from an older draft becomes useful again. Without proper organization, finding those changes would be very difficult.

Programming works in a similar way. Code changes over time, and developers often need to revisit old code. **Git** helps manage these changes, and the `git diff` command is a powerful tool for comparing differences across files, commits, and branches.

---

## git status vs git diff
- **git status**
  - Shows *which files* have been changed
  - Does NOT show what changed inside the files

- **git diff**
  - Shows *exactly what has changed* inside files
  - Displays added and removed lines

You can think of it like this:
- `git status` → shows file names
- `git diff` → opens the file and shows content differences

---

## Basic Concept of git diff
The `git diff` command compares:
- Previous version vs current version of a file
- One commit vs another commit
- One branch vs another branch

It highlights:
- Removed lines (prefixed with `-`)
- Added lines (prefixed with `+`)

---

## Simple Example (File Comparison)
Imagine a file named `CITIES.txt` that lists cities you visited.

- You updated the file during a tour
- Later, you forgot what you changed

Running:
```bash
git diff
