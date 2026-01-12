# Installing Git on Mac

## Overview
- Git works on all major operating systems:
  - Windows
  - macOS
  - Linux
- On macOS, Git is often installed by default
- Git is mainly used through the command line
- Git integrates well with IDEs and GUI tools

---

## Check if Git Is Already Installed
Before installing Git, check whether it is already available on your Mac.

Command:
- `git --version`

- If a Git version is displayed, Git is already installed
- If you see **command not found**, Git needs to be installed

---

## Installing Git Using Xcode

### About Xcode
- Xcode is Apple’s official development environment
- Git comes bundled with Xcode
- Xcode uses a large amount of disk space
- There are lighter alternatives if you only want Git

---

### Option 1: Install Full Xcode
- Download Xcode from:
  https://developer.apple.com/xcode/
- After installation, open Terminal and verify Git:

Command:
- `git --version`

Example output:
- `git version 2.30.1 (Apple Git-130)`

---

### Option 2: Install Xcode Command Line Tools (Recommended)
- This is a lightweight alternative to full Xcode
- Install directly from Terminal

Command:
- `xcode-select --install`

- The installation will begin, or
- You may see a message saying Git is already installed

Verify installation:
- `git --version`

---

## Configure Git User Information (Optional)
After installing Git, configure your user details:

Commands:
- `git config --global user.name "Your Name"`
- `git config --global user.email "your.email@example.com"`

These details are used in commit history.

---

## Installing Git Using Homebrew

### What Is Homebrew?
- Homebrew is a popular package manager for macOS
- Makes installing software simple

---

### Install Homebrew
- Visit:
  https://brew.sh/
- Follow the installation instructions for macOS

---

### Install Git with Homebrew
Once Homebrew is installed, run:

- `brew install git`

Verify installation:
- `git --version`

---

## Key Points
- Git may already be installed on macOS
- Xcode Command Line Tools are the recommended lightweight option
- Homebrew provides an easy alternative installation method
- Always verify installation using `git --version`
- Git user configuration helps identify commits
