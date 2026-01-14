# Branches

## Overview
- Branches allow developers to work on features or fixes independently
- Changes in a branch do not affect the main branch until merged
- Branching makes collaboration cleaner and safer

---

## Checking the Current Repository
- Open the terminal
- Verify the current directory:

pwd

- Ensure you are inside the repository (example: `my-first-repo`)
- Check repository status:

git status

- If up to date, Git shows:
  - Branch: `main`
  - Status: up to date with `origin/main`
  - Working tree clean

---

## Creating a New Branch
- Create and switch to a new branch:

git checkout -b feature/lesson

- This command:
  - Creates a new branch
  - Switches from `main` to `feature/lesson`

### Alternative Method
- Create a branch only:

git branch feature/lesson

- This does **not** switch branches
- To switch manually:

git checkout feature/lesson

---

## Verifying the Active Branch
- Check available branches:

git branch

- The active branch is marked with `*`
- All changes now apply only to `feature/lesson`

---

## Branch Isolation
- The `main` branch is unaware of changes in `feature/lesson`
- Even after pushing, branches remain separate
- Changes must be merged back into `main`

---

## Adding Changes to the Branch
- Create a new file:

touch test2.txt

- Stage the file:

git add test2.txt

- Commit the change:

git commit -m "add test2.txt file"

---

## Pushing the Branch to GitHub
- Push the branch to the remote repository:

git push -u origin feature/lesson

- `-u` sets upstream tracking
- GitHub now recognizes the new branch
- HTTPS users will be prompted for credentials

---

## Creating a Pull Request
- Open GitHub in a browser
- GitHub displays a prompt for the new branch
- Click **Compare & pull request**
- Pull request:
  - Requests review of changes
  - Compares `feature/lesson` with `main`
  - Shows file differences (example: `test2.txt`)
- Click **Create pull request**

---

## Reviewing and Merging
- Team reviews the pull request
- Changes may be approved or declined
- Once approved:
  - Merge into the `main` branch
- Optionally delete the branch after merging

---

## Updating Local Main Branch
- Switch back to main:

git checkout main

- Pull the latest changes:

git pull

- Verify files:

ls

- `test2.txt` is now present in `main`

---

## Branch Naming Conventions
- Feature branches:
  - `feature/lesson`
- Bug fixes:
  - `fix/bug-name`
- Teams decide naming standards
- No limit on the number of branches

---

## Key Points
- Branches isolate work
- `git checkout -b` creates and switches branches
- Pull requests review and merge changes
- Independent branches reduce conflicts
- Branch-based workflows are essential for collaboration
