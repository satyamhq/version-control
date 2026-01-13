# Creating and Cloning a Repository

## Creating a Repository on GitHub
- Log in to the GitHub website
- Click the green **Create repository** button
- On the “Create a new repository” page:
  - Select your account as the **owner**
  - Enter a repository name (example: `my-first-repo`)
    - A green tick indicates the name is available
    - An X indicates the name must be changed
  - Add a description (example: *practice account for learning Git*)
  - Choose repository visibility:
    - **Public**: Anyone can view the repository
    - **Private**: Only users you grant access to can view it

---

## Initializing the Repository
- Choose initialization options:
  - README file
  - `.gitignore` file
  - License
- For this example, select **Initialize with a README**
- Click **Create repository**

---

## Repository Structure
- The repository is created with:
  - A `README.md` file
  - A default **main branch**
- `README.md` uses Markdown format
  - Used for documentation
  - Supports headings, text, images, and formatting
- Every repository starts with a single main branch (main line)

---

## GitHub Repository Options
- **Go to file**: Browse repository files
- **Add file**: Add new files via GitHub UI
- **Code** button:
  - HTTPS clone URL
  - SSH clone URL
  - GitHub CLI option
  - GitHub Desktop option
  - Download ZIP option

---

## Cloning a Repository Using HTTPS
- Click the **Code** button
- Select **HTTPS**
- Copy the HTTPS URL

---

## Preparing Local Workspace
- Open the terminal
- Navigate to your home directory
- Create a directory for repositories:

mkdir projects

- Move into the directory:

cd projects

---

## Cloning the Repository
- Run the clone command:

git clone <HTTPS_URL>

- Git displays messages showing:
  - Objects being downloaded
  - Progress reaching 100%
  - Completion confirmation

---

## Verifying the Clone
- List directory contents:

ls -la

- The cloned repository folder appears
- Navigate into the repository:

cd my-first-repo

- List files:

ls -la

- Files present:
  - `README.md`
  - `.git` directory (used by Git for version control)

---

## Key Points
- Repositories can be public or private
- README.md is commonly used for documentation
- HTTPS cloning requires authentication
- The `.git` folder tracks version history
- Cloning creates a local copy of the remote repository
