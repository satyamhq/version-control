# Connecting to GitHub via SSH

## Overview
- SSH (Secure Shell) is the recommended way to authenticate with GitHub from a local device
- Uses a **public and private key pair**
- Eliminates the need to enter username and password repeatedly
- Authentication happens automatically using SSH keys
- Keys are generated on the local machine and the public key is added to GitHub

---

## Generate SSH Keys
- The process is the same for Windows and macOS
- Windows: Use **Git Bash**
- macOS: Use **Terminal**

### Step 1: Open Terminal
Run the following command:

ssh-keygen -t ed25519 -C "your@email.com"

- Replace the email with your GitHub email
- Press **Enter**

---

### Step 2: Passphrase
- When prompted for a passphrase:
  - Press **Enter** to skip
  - Press **Enter** again to confirm

---

### Step 3: Key Generation
- A public and private key pair is generated
- Keys are stored in the `.ssh` directory

Files created:
- Private key → kept secret
- Public key → ends with `.pub`

---

## Locate the SSH Key
List the SSH directory:

ls ~/.ssh/

- Identify the public key file (ends with `.pub`)

---

## Copy the Public Key

### macOS:
pbcopy < ~/.ssh/<YOUR_KEY>.pub

### Windows:
cat ~/.ssh/<YOUR_KEY>.pub | clip

- Replace `<YOUR_KEY>` with the actual key filename
- The public key is now copied to your clipboard

---

## Add SSH Key to GitHub

### Step 1: Log in to GitHub
- Sign in to your GitHub account

---

### Step 2: Open Settings
- Click the profile icon (top-right)
- Select **Settings**

---

### Step 3: SSH and GPG Keys
- In the left sidebar, under **Access**
- Click **SSH and GPG Keys**

---

### Step 4: Add New SSH Key
- Click **New SSH key**

---

### Step 5: Enter Key Details
- Enter a title (e.g., "My Laptop")
- Paste the public key into the key field

---

### Step 6: Save Key
- Click **Add SSH key**

---

## Accessing Repositories
- When using SSH authentication:
  - Always use the **SSH URL** of the repository
- SSH URLs usually start with:
  - `git@github.com:`

---

## Key Points
- SSH is more secure and convenient than HTTPS passwords
- Public key is added to GitHub, private key stays local
- No repeated credential entry required
- Always use the SSH repository address
- SSH keys can be reused across repositories
