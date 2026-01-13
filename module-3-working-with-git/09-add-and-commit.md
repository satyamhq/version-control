# Add and Commit

## Checking the Current Repository
- Open the terminal
- Check the current directory using:

pwd

- Confirm you are inside the repository (example: `my-first-repo`)
- List all files, including hidden files:

ls -la

- Files present:
  - `README.md`
  - `.git` (hidden folder used by Git)

---

## Checking Repository Status
- Before making changes, always check the current status:

git status

- This command shows:
  - Current branch (example: `main`)
  - Whether the branch is up to date with `origin/main`
  - Whether there are files to commit
- Message **“working tree clean”** means no changes exist

---

## Creating a New File
- Create a new file:

touch test.txt

- Check status again:

git status

- Git reports:
  - `test.txt` is **untracked**
  - File is not yet part of version control

---

## Staging Files (git add)
- To tell Git to track the file, add it to the staging area:

git add test.txt

- Check status:

git status

- File is now:
  - **Tracked**
  - **Staged** and ready to be committed

---

## Unstaging a File
- To remove a file from the staging area:

git restore --staged test.txt

- Check status again:

git status

- File returns to **untracked** state

---

## Re-Adding the File
- Add the file again:

git add test.txt

- Confirm it is staged:

git status

---

## Understanding the Staging Area
- The staging area prepares files for commit
- Allows you to control exactly what goes into a commit
- All changes are **local only**
- Nothing is shared with GitHub until a push is performed

---

## Committing Changes
- Commit staged files with a message:

git commit -m "adding a new file for testing"

- Git confirms:
  - Number of files changed
  - Creation of `test.txt`

---

## Final Status Check
- Run status again:

git status

- Output shows:
  - Nothing to commit
  - Working tree clean
- Git提示 indicates local commits exist and can be published using `git push`

---

## Key Points
- `git status` checks repository state
- `git add` stages files
- `git restore --staged` unstages files
- `git commit` saves changes locally
- Commits stay local until pushed to remote
- Staging helps organize clean commits
