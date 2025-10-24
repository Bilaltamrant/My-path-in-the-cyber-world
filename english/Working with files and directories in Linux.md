
# 📚 Working with Files and Directories in Linux

**Date:** [October 24, 2025]  
**Level:** Beginner  
**Status:** 🟢 Completed

---

## 🎯 Goals / Objectives

* Learn how to create files and directories using the terminal.
* Gain practical skills in navigating, copying, renaming, and deleting within the Linux system.

---

## 📝 Summary & Core Concepts

This lesson explains how to manage files and directories in Linux using the terminal. It covers commands for creation, moving, copying, and renaming, along with displaying the file structure in a tree format. These skills are essential for any Linux user who wants to control the system without a graphical interface.

### 📑 Key Concepts
* **touch:** Creates an empty file.
* **mkdir:** Creates a new directory.
* **mv:** Moves or renames files.
* **cp:** Copies files.
* **tree:** Displays the file structure in a tree format.

---

## ⚙️ Practical Commands & Examples

### 1. Create an empty text file

**Description:** Creates a file with no content.

```bash
touch info.txt
```

---

### 2. Create a directory

**Description:** Creates a new directory with a specified name.

```bash
mkdir storage
```

---

### 3. Create nested directories in one command

**Description:** Creates a chain of directories even if they don’t exist yet.

```bash
mkdir -p Storag/local/user/documents
```

---

### 4. Display file and directory structure

**Description:** Shows files and folders in a tree-like format within the current path.

```bash
tree .
```

---

### 5. Create a file inside a specific directory

**Description:** Creates a file at a specified path inside a folder.

```bash
touch ./filename/path
```

---

### 6. Rename a file

**Description:** Changes the file name from `info.txt` to `information.txt`.

```bash
mv info.txt information.txt
```

---

### 7. Move a file to another directory

**Description:** Moves the file to a new folder.

```bash
mv information.txt storage/
```

**Move multiple files:**

```bash
mv file1 file2 /storage
```

---

### 8. Copy a file to another directory

**Description:** Copies a file from one path to another.

```bash
cp /home/kali/Downloads/ssd /home/kali/Desktop/folder/
```

---

## 📊 Outcomes & Key Takeaways

* **Positive Result:** Successfully created files and directories and navigated between them using the terminal.
* **Challenge Faced:** Typing long paths accurately, solved using auto-completion.
* **Core Lesson:** Understanding the file structure in Linux makes system management easier and more efficient.

---

## 🔗 Keywords & Resources

### 🏷️ Keywords / Tags
`Linux`, `File_System`, `Directories`, `mv`, `cp`, `mkdir`, `touch`, `tree`, `CLI`

### 📚 Further Reading
1. [Linux Command Line Basics](https://linuxcommand.org/)
2. [The Linux Command Line Book](https://linuxcommand.org/tlcl.php)
