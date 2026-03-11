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
