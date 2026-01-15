# Git Push and Pull
## Overview
After using `git add` and `git commit` to record changes in your **local repository**, the next step is to synchronize those changes with a **remote repository** (such as GitHub).  
This is done using the commands:

- `git push` → Upload local commits to the remote repository  
- `git pull` → Download and merge remote changes into the local repository  

Git follows a **distributed workflow**, meaning you can work offline and only interact with the remote repository when pushing or pulling changes.

---

## Checking Repository Status
Before pushing or pulling, always check your current state:

```bash
git status
