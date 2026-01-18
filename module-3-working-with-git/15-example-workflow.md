# Example Workflow – Git & Feature Branching

## What is a Workflow?
A **workflow** is a structured sequence of steps used to complete a task efficiently and consistently.

### Real-life Example
Applying for a job is a workflow:
1. Prepare your resume  
2. Search for jobs  
3. Submit applications  
4. Prepare for interviews  

In **computer programming**, workflows play a crucial role in guiding developers on how to work together on projects.

---

## Why Workflows Are Important
- Provide clear guidance to team members  
- Prevent conflicts and blockers in development  
- Ensure smooth testing and deployment  
- Maintain consistency and code quality  
- Help multiple developers collaborate efficiently  

Choosing the right workflow depends on:
- Team size  
- Workplace culture  
- Type of product being developed or updated  

---

## Basic Development Workflow Example
As a developer working on a project:
1. Pull the project from a **remote repository** to your local machine  
   (also called *checking out* or *pulling* a project)
2. Build and run the project locally  
3. Make changes to the code  
4. Push the changes back to the remote repository  
5. Other developers can now see and use your changes  

**Purpose of a workflow:**  
To guide you and your team without disrupting testing, deployment, or other developers’ work.

---

## Feature Branch Workflow
**Feature branching** is one of the most commonly used workflows.

### What is Feature Branching?
- A new branch is created from the **main branch**
- Work for a specific feature or task is done only on this branch
- The **main branch remains stable** and unchanged
- Changes are merged into the main branch only after review

---

## Key Concepts
- **Main Branch**: Source of truth for the application  
- **Feature Branch**: A dedicated branch for a specific feature or task  
- **Pull Request (PR)**: A request to merge changes into the main branch  
- **Code Review**: Peer review of changes before merging  

---

## Feature Branch Workflow Steps (Using Git)

### Step 1: Get the Latest Code
Always ensure your local repository is up to date:
```bash
git pull
