# How Git Works

## Git and GitHub Overview
- GitHub is a **cloud-based hosting service** for Git repositories
- Acts like a social platform for developers
- Users can:
  - Follow other users
  - Share repositories
  - Accept code contributions from anywhere in the world
- Git is used locally through:
  - Git Bash (Windows)
  - Terminal (macOS)

---

## Working with a Local Repository
- Navigate to the cloned repository:

cd my-first-repo

- List all files, including hidden files:

ls -la

- Important items in the repository:
  - `README.md` → Documentation file created on GitHub
  - `.git` → Hidden folder used by Git to track changes

---

## The .git Folder
- `.git` is a **hidden directory**
- Any file or folder starting with `.` is hidden in Linux/macOS
- This folder stores:
  - Version history
  - Configuration
  - Commit data
- Automatically created when:
  - A repository is initialized with `git init`
  - Or cloned from GitHub
- No need to run `git init` when cloning from GitHub

---

## Git Workflow
Git follows a workflow with **three main states**:

### 1. Modified
- Files are:
  - Added
  - Updated
  - Deleted
- Git detects changes but does not track them yet

---

### 2. Staged
- Files are added to the **staging area**
- Git starts tracking changes
- Acts as a checkpoint before committing
- Provides control over what gets saved

---

### 3. Committed
- Changes are permanently saved
- Git creates a snapshot of the project
- Similar to a save point

---

## Complete Git Workflow Example
1. File is created or modified in the **working directory**
2. File is added to the **staging area**
3. Changes are **committed** locally
4. Commit is **pushed** to the remote repository
5. Other users can:
   - Fetch
   - Merge
   - Check out changes into their working directory

---

## Key Points
- `.git` controls version tracking
- `README.md` documents the project
- Git tracks changes in stages
- Modified → Staged → Committed
- Remote repositories allow collaboration
- Understanding the workflow is essential for Git usage

---

You now understand **how Git works**, what is inside a Git repository, and how the **Git workflow** functions.
