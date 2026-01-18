# Forking
## Introduction
In previous lessons, you learned about workflows such as **branching**, where multiple developers work on different branches of the **same repository**.  
**Forking** is another important workflow, especially common in open-source projects.

The key difference is:
- **Branching** → creates new branches inside the same repository  
- **Forking** → creates an entirely new repository under a different account  

---

## Branching vs Forking
### Branching
- All team members work within **one shared repository**
- New branches are created from the same repo
- Requires write access to the repository
- Common in internal or private team projects

### Forking
- Creates a **new copy of the repository** in your own GitHub account
- Original repository remains untouched
- No write access to the original repo is required
- Common in open-source and public projects

---

## How Forking Works (Concept)
Imagine a repository called **coolgame**.

- Joe forks the `coolgame` repository
- A **complete copy** (including full history) is created in Joe’s GitHub account
- Joe can freely modify the repository without affecting the original
- The original owner continues working normally, unaware of Joe’s changes

To contribute back:
- Joe creates a **Pull Request (PR)** from his fork
- The PR compares Joe’s repository with the original repository
- The original owner reviews and decides whether to accept or reject the changes

---

## Forking Workflow Overview
1. Fork the original repository
2. Clone the forked repository locally
3. Create a new branch
4. Make changes and commit them
5. Push changes to your fork
6. Create a Pull Request to the original repository
7. Repository owner reviews and merges (or rejects)

---

## Forking a Repository on GitHub

### Step 1: Open the Repository
- Go to the GitHub repository you want to fork

### Step 2: Click Fork
- Click the **Fork** button at the top-right corner of the page

### Step 3: Choose Destination
- Select the GitHub account where you want the fork to live

### Step 4: Repository Is Forked
- GitHub creates a full copy in your account
- The repository is now yours to modify

On the repository page, GitHub will display:
- “Forked from `<original-owner>/<repository-name>`”

---

## Forked Repository UI Differences
- GitHub shows the fork is **up to date** with the original repository
- A **Fetch upstream** option appears
  - Used to pull updates from the original repository
- You can sync changes without affecting the original project

---

## Example: Working with a Fork

### Step 1: Clone the Forked Repository
```bash
git clone <your-fork-url>
