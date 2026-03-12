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


