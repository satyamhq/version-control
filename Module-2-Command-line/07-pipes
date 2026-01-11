# Pipes

## Navigating to the Files
First, the terminal is launched and the contents of the current directory are checked using the `ls` command.

ls

This shows two folders: `archive` and `projects`.

To move into the `archive` directory:

cd archive

Then list its contents:

ls

This reveals a folder named `submissions`.

To move into the `submissions` directory:

cd submissions

Now check what files are inside:

ls

The output shows two files: `file1.txt` and `file2.txt`.  
Both files contain text data.

---

## Viewing File Contents
To view the contents of a file, the `cat` command is used.

cat file1.txt

This command prints the contents of `file1.txt` directly to the terminal.

---

## Word Count Command
The word count command is abbreviated as `wc`.

To count the number of words in a file, use the `-w` flag:

wc -w file1.txt

The output shows that `file1.txt` contains **181 words**.

---

## Using Pipes
A pipe (`|`) allows the output of one command to be used as the input of another command.

### Example 1: Counting Files in a Directory
The `ls` command outputs file names. This output can be piped into `wc`.

ls | wc -w

This returns `2`, because there are two files in the directory.

---

## Using Pipes with File Content
To find the word count of a file using pipes:

cat file1.txt | wc -w

This returns a word count of **181** for `file1.txt`.

---

## Using Pipes with Multiple Files
Multiple files can be combined using `cat` and then piped into `wc`.

cat file1.txt file2.txt | wc -w

This command outputs a total word count of **362**, which is the combined word count of both files.

---

## Summary
- `cat` displays file contents  
- `wc -w` counts words in a file  
- `|` (pipe) passes output from one command to another  
- Pipes allow powerful command combinations  
- Multiple files can be processed together using pipes  

You have now learned how to use **pipes** to process and analyze file data efficiently using the command line.
