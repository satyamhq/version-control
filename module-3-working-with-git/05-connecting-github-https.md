# Connecting to GitHub via HTTPS

## Overview
- When using GitHub via platforms like Coursera, authentication over **HTTPS** is required
- Authentication is done using a **Personal Access Token (PAT)**
- A Personal Access Token acts as a password replacement
- Tokens can be:
  - Revoked at any time
  - Set with an expiry date
- This improves account security

---

## What Is a Personal Access Token
- A secure token used instead of your GitHub account password
- Required for HTTPS-based Git operations
- Can be limited by scope and expiry
- If lost, it must be regenerated

---

## Generating a Personal Access Token

### Step 1: Log in to GitHub
- Sign in to your GitHub account

---

### Step 2: Open Settings
- Click your **profile icon** (top-right)
- Select **Settings**

---

### Step 3: Open Developer Settings
- In the left sidebar, click **Developer settings**

---

### Step 4: Personal Access Tokens
- Click **Personal access tokens**
- Select **Tokens (classic)**
- Click **Generate new token**
- Choose **Generate new token (classic)**

---

### Step 5: Token Details
- Enter a **token name**
- Set an **expiry time**
  - Choose *No expiration* if you plan to revoke it manually

---

### Step 6: Select Scopes
- Under scopes, select:
  - `repo`
- This allows access to repositories

---

### Step 7: Generate Token
- Scroll down
- Click **Generate token**

---

### Step 8: Save the Token
- Copy the generated token immediately
- Store it securely
- The token will not be visible again after leaving the page

> If the token is lost, delete it and generate a new one.

---

## Accessing Repositories via HTTPS
- Ensure you have permission to access the repository
- Use the **HTTPS URL** of the repository
- When prompted for credentials:
  - Username → GitHub username
  - Password → Personal Access Token

---

## Key Points
- HTTPS authentication requires a Personal Access Token
- Tokens improve security compared to passwords
- Always save the token after creation
- Use the repository’s HTTPS URL for access
- Tokens can be revoked or regenerated anytime
