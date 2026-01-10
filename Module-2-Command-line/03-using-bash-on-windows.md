# Using Bash on Windows

## Navigating the Home Directory

After opening the terminal window, the first step is to navigate to the home directory. This can be done using the `cd` command followed by a tilde (`~`), which represents the home directory.

Example:
cd ~

To view all files in the directory, including hidden files, the following command is used:
ls -la

This command lists all files in a detailed format, including hidden files.

---

## Understanding .bashrc and .bash_profile

After listing the files, two important configuration files may appear:
- .bashrc
- .bash_profile

### .bashrc File

The `.bashrc` file is primarily used for shell configuration. It is a script that runs every time a new terminal session starts.

To view the contents of the file:
less .bashrc

The `.bashrc` file may contain:
- Shell color configurations
- Command history settings
- Aliases and custom shell behavior

To exit the `less` viewer, press the `q` key.

---

### .bash_profile File

The `.bash_profile` file is commonly used to set environment variables needed for development.

To view the file:
less .bash_profile

This file may contain:
- Environment variables such as JAVA_HOME or PYTHON_HOME
- Path configurations required for development tools

Press `q` to exit the file view.

---

## Creating a Simple Bash Script

To create a shell script, a text editor is required. In this example, Vim is used.

Create and open a new file:
vim testshell.sh

---

## Writing the Bash Script

Press `i` to enter insert mode. At the top of the file, specify the script type using a shebang line.

Example:
#!/bin/bash

This tells the operating system that the file is a Bash script.

To print text to the terminal, use the `echo` command:
echo HelloWorld

Press `Esc` to exit insert mode, then save and quit the file by typing:
:wq!

Press Enter to confirm.

---

## Making the Script Executable

After creating the file, it exists but is not executable. To change its permissions, the `chmod` command is used.

Set executable permissions:
chmod 755 testshell.sh

To confirm the change, list files again:
ls -la

The file will now show executable permissions.

---

## Running the Bash Script

To run the script, use the following command:
./testshell.sh

Once executed, the text "HelloWorld" will be printed to the terminal.

---

## Key Takeaways

- The home directory can be accessed using `cd ~`
- `.bashrc` is used for shell configuration
- `.bash_profile` is used for environment variables
- Vim can be used to create and edit Bash scripts
- Scripts must be given executable permissions using `chmod`
- Executable scripts can be run directly from the command line
