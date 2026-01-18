# Git Blame 
## Introduction
One day, you might be managing a large team of developers. Keeping track of **who changed what, when, and why** can become very complex.  
Git solves this problem by maintaining a complete history of every file. One of the most useful commands for this purpose is **`git blame`**.

The `git blame` command helps identify:
- Who made a change
- When the change was made
- Which commit introduced the change
- Which exact line was affected

---

## Purpose of git blame
Git blame is used to:
- Track responsibility for each line of code
- Understand the history of a specific file
- Find when and by whom a bug or change was introduced
- Audit changes in collaborative projects

Git already records history, and `git blame` allows you to **inspect that history line by line**.

---

## What git blame Shows
For every line in a file, `git blame` displays:
- **Commit ID (hash)** – identifies the commit where the line was last changed  
- **Author** – the developer who made the change  
- **Timestamp** – date and time of the commit  
- **Line number** – position of the line in the file  
- **Content** – the actual code or text on that line  

The same commit ID may appear multiple times if several lines were changed in one commit.

---

## Basic Usage of git blame
To run git blame on a file:
```bash
git blame filename
