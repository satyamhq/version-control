# Grep

## Overview
- **Grep** stands for **Global Regular Expression Print**
- Used to search:
  - Inside files
  - Across folders
  - Through command output
- Matches lines containing a given pattern

---

## Basic Grep Search
- Grep searches for a pattern inside a file

Example:
- `grep Sam names.txt`
- Returns names that begin with **Sam**

---

## Case Sensitivity
- Grep is **case-sensitive** by default

Example:
- `grep sam names.txt`
- Returns different results because lowercase `sam` does not match uppercase `Sam`

---

## Ignoring Case Sensitivity (`-i`)
- The `-i` flag ignores case differences

Example:
- `grep -i Sam names.txt`
- Returns:
  - Names starting with `Sam`
  - Names containing `sam` anywhere in the word

---

## Exact Word Match (`-w`)
- The `-w` flag matches the exact word only
- Partial matches are ignored

Example:
- `grep -w Sam names.txt`
- Returns only the exact name **Sam**

---

## Using Grep with Pipes
- Grep can filter the output of other commands using a pipe (`|`)

Example:
- `ls /bin`
- Lists all executable files in `/bin`

Filtered search:
- `ls /bin | grep zip`
- Returns only files related to `zip`

---

## Refining Searches
- Grep supports:
  - Case-insensitive searches (`-i`)
  - Exact matches (`-w`)
  - Partial matches
- Flags can be combined with pipes for precise results

---

## Key Points
- Grep searches text patterns
- Case-sensitive by default
- `-i` ignores case
- `-w` matches exact words
- Pipes enhance filtering
- Useful for searching files, directories, and command outputs
