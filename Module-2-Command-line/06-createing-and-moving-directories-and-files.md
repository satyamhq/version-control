# Creating and Moving Directories and Files

## Checking the Current Directory
To check the current directory, use the `pwd` (Print Working Directory) command.

pwd

If the output is `/`, it means you are in the root directory.

---

## Listing Directory Contents
To list the contents of the current directory in detailed format, use:

ls -l

Initially, the root directory contains a directory named `projects`.

---

## Creating a New Directory
To create a new directory, use the `mkdir` (make directory) command.

mkdir submissions

After creating the directory, list the contents again to verify:

ls -l

A new directory named `submissions` will appear.

---

## Navigating into a Directory
To move into the newly created directory:

cd submissions

To check its contents:

ls

The directory is empty at this point.

---

## Creating Files
To create a new text file, use the `touch` command.

touch test1.txt

To create another file:

touch test2.txt

Now list the contents in detailed format:

ls -l

Both `test1.txt` and `test2.txt` will be displayed inside the `submissions` directory.

---

## Returning to the Parent Directory
To go back to the root directory:

cd ..

Verify by listing contents:

ls -l

Both `projects` and `submissions` directories are now visible.

---

## Creating Another Directory
Create a new directory named `archive`:

mkdir archive

Verify all directories:

ls -l

The directories `archive`, `projects`, and `submissions` are now present.

---

## Clearing the Terminal Screen
To clear the terminal screen:

clear

Then list the contents again:

ls -l

---

## Moving a Directory
To move the `submissions` directory into the `archive` directory, use the `mv` (move) command:

mv submissions archive

Verify the move:

ls -l

The `submissions` directory will no longer appear in the root directory.

---

## Verifying the Moved Directory
Navigate into the `archive` directory:

cd archive

List the contents:

ls -l

The `submissions` directory is now inside `archive`.

---

## Verifying Moved Files
Navigate into the `submissions` directory:

cd submissions

List the contents:

ls -l

The files `test1.txt` and `test2.txt` are present, confirming they were moved along with the directory.

---

## Summary
- `pwd` checks the current directory  
- `ls -l` lists contents in detailed format  
- `mkdir` creates directories  
- `cd` changes directories  
- `touch` creates files  
- `mv` moves files or directories  
- `clear` clears the terminal screen  

You have successfully learned how to create directories and files, and move them using the command line.
