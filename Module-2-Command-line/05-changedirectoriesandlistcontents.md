# Change Directories and List Contents

## Checking the Current Directory
The `pwd` command (Print Working Directory) is used to display the current directory.

pwd

If the output is `/`, it means you are in the root directory. The root directory is the top-level directory in the operating system.

## Listing Directory Contents
The `ls` command (list) displays the contents of the current directory.

ls

This shows the names of files and directories inside the current directory.

## Using Flags with ls
Flags are used to modify the behavior of commands.

Using the `-l` flag with `ls` prints the output in a detailed list format.

ls -l

This displays file permissions, owner, group, size, date, and name.

## Understanding File Types
The first character in the `ls -l` output represents the file type:

l  → Link file  
d  → Directory  
-  → Standard file (text or configuration file)

Example:
- A link file may appear as `temp -> tmp`, meaning `temp` points to the `tmp` directory.
- Directories such as `bin` and `etc` are shown with `d`.
- Files like `resolv.conf` are shown with `-`.

The owner and group fields indicate who owns the file and which group it belongs to.

## Changing Directories
To move into another directory, use the `cd` command.

cd etc

To confirm the current directory:

pwd

## Viewing Directory Contents
After changing directories, the contents can be viewed using:

ls  
ls -l

Each directory contains different files and subdirectories.

## Moving to the Parent Directory
To move up one level in the directory structure, use:

cd ..

Example:
- From `/etc` back to `/`
- From `/etc/ssh` back to `/etc`

## Using Absolute Paths
An absolute path starts from the root directory.

cd /

This command moves directly to the root directory from any location.

## Navigating Multiple Directories
Example navigation:

cd etc  
ls  
cd ssh  
ls  
cd ..  
cd ..  
pwd

This sequence moves from root to `etc`, then to `ssh`, and back to root.

## Conclusion
The `pwd`, `ls`, and `cd` commands are essential for navigating the file system. Understanding directory structure, file types, and paths helps efficiently move through and manage files in a command-line environment.
