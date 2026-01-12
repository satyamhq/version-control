# Redirection

## Overview
- Every Linux command takes input and produces output  
- By default:
  - Standard input → Keyboard  
  - Standard output → Screen  
  - Standard error → Screen  
- Redirection allows changing the input and output sources

---

## Types of Redirection
The shell assigns numbers to input/output streams:

- `0` → Standard Input  
- `1` → Standard Output  
- `2` → Standard Error  

---

## Standard Input Redirection
- Standard input normally comes from the keyboard  
- The `<` symbol is used for input redirection  

### Using cat to Take Input from Keyboard
- `cat > input.txt`
- Type text into the terminal
- Press **Ctrl + D** to end input

### Reading Input from a File
- `cat < input.txt`
- Displays the contents of `input.txt`

---

## Standard Output Redirection
- Output normally goes to the screen  
- The `>` symbol redirects output to a file  

Example:
- `ls -l > output.txt`

To view the output:
- `less output.txt`

---

## Standard Error Redirection
- Errors are sent to standard error  
- The `2>` symbol redirects errors to a file  

Example:
- `ls -l /bin/usr 2> error.txt`

To view the error:
- `less error.txt`

---

## Redirecting Output and Error Together
- Both standard output and error can be redirected to the same file  

Example:
- `ls -l /bin/usr > error_output.txt 2>&1`

To view the file:
- `less error_output.txt`

---

## Key Symbols
- `<`  → Input redirection  
- `>`  → Output redirection  
- `2>` → Error redirection  
- `2>&1` → Redirect error to output  

---

## Key Points
- Redirection changes where input and output go  
- Standard streams are identified by numbers  
- Errors must be redirected separately  
- Useful for logging and automation  
