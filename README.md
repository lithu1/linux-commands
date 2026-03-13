# linux-commands
# Linux Commands Notes

## Day 1 – Basic Linux Commands

### 1. **pwd** (Print Working Directory)

Shows the current directory you are working in.

```bash
pwd
```

---

### 2. **ls** (List Files and Directories)

Displays files and folders in the current directory.

```bash
ls
```

Common options:

```bash
ls -l
```

Shows detailed information (permissions, owner, size).

```bash
ls -a
```

Shows hidden files.

---

### 3. **cd** (Change Directory)

Used to move between directories.

```bash
cd foldername
```

```bash
cd ..
```

Moves one directory back.

```bash
cd ~
```

Moves to the home directory.

---

### 4. **mkdir** (Make Directory)

Creates a new folder.

```bash
mkdir foldername
```

Example:

```bash
mkdir devops-practice
```

---

### 5. **touch**

Creates a new empty file.
Note: It creates the file but **does not open it**.

```bash
touch filename.txt
```

Example:

```bash
touch notes.txt
```

---

### 6. Opening / Viewing Files

**nano** – Simple text editor

```bash
nano file.txt
```

**vim** – Advanced text editor

```bash
vim file.txt
```

**cat** – Display file content

```bash
cat file.txt
```

**less** – View large files page by page

```bash
less file.txt
```




## Day 2 – File Operations

### 1. **cp** (Copy Files or Directories)

Used to copy files or directories from one location to another.

```bash
cp source destination
```

Example:

```bash
cp file1.txt file2.txt
```

Creates a copy of **file1.txt** named **file2.txt**.

Copy a directory:

```bash
cp -r folder1 folder2
```

`-r` means recursive (copies the folder and everything inside it).

---

### 2. **mv** (Move or Rename Files)

Used to move files to another directory or rename them.

Rename a file:

```bash
mv oldname.txt newname.txt
```

Move a file:

```bash
mv file.txt Documents/
```

Note: **mv moves the original file, it does not create a copy.**

---

### 3. **rm** (Remove Files or Directories)

Used to delete files or directories.

Delete a file:

```bash
rm file.txt
```

Delete a directory:

```bash
rm -r foldername
```

Force delete:

```bash
rm -f file.txt
```

Explanation:

* **-r** → recursive delete (for directories)
* **-f** → force delete without confirmation

⚠️ Be careful because deleted files cannot be easily recovered.

---

### 4. **echo**

Used to print text to the terminal or write text into a file.

Print text:

```bash
echo "Hello Linux"
```

Write text into a file:

```bash
echo "Learning Linux" > notes.txt
```

Note: `>` overwrites the existing file content.

---

### 5. **clear**

Used to clear the terminal screen.

```bash
clear
```

This removes previous commands from the screen and gives a clean terminal.



## Day 3 – File Inspection Commands

### 1. **head** (View Beginning of File)

Displays the first few lines of a file.
By default, it shows the first **10 lines**.

```bash
head file.txt
```

Show the first 5 lines:

```bash
head -n 5 file.txt
```

---

### 2. **tail** (View End of File)

Displays the last few lines of a file.
By default, it shows the last **10 lines**.

```bash
tail file.txt
```

Show the last 5 lines:

```bash
tail -n 5 file.txt
```

Follow a file in real time (commonly used for logs):

```bash
tail -f app.log
```

---

### 3. **wc** (Word Count)

Used to count the number of **lines, words, and characters** in a file.

```bash
wc file.txt
```

Example output:

```
10  50  300 file.txt
```

Meaning:

* 10 lines
* 50 words
* 300 characters

Count only lines:

```bash
wc -l file.txt
```

---

### 4. **history**

Displays a list of previously executed commands in the terminal.

```bash
history
```

Run a command again using its number:

```bash
!5
```

This executes command number **5** from the history list.

---

### 5. **man** / **--help**

Used to view the manual or help documentation for commands.

Example using `man`:

```bash
man ls
```

If `man` is not available (like in Git Bash), use:

```bash
ls --help
```

Press **q** to exit the manual page.


