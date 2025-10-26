# 📚 Searching for Files and Directories in Linux

**Date:** 2025-10-26  
**Level:** Intermediate  
**Status:** 🟢 Completed

---

## 🎯 Goals / Objectives

* Understand the difference between the `which` and `find` search tools in Linux.  
* Learn how to use search commands to locate executable programs and general files with advanced filtering.

---

## 📝 Summary & Core Concepts

In this lesson, I learned how to use search tools in Linux to locate programs and files. The `which` command helps identify the location of executable programs, while `find` allows advanced searching using criteria like type, size, date, and ownership.

### 📑 Key Concepts
* **which:** Searches for the path of an executable program listed in system environment variables.  
* **find:** Searches the system for files or directories and supports powerful filtering by type, name, size, date, and user.

---

## ⚙️ Practical Commands & Examples

### 1. Using `which` to locate an executable program

**Description:** We use the `which` command to check if a program like `python` is installed and where it resides.

```bash
which python
```

**Expected Output:**
```bash
/usr/bin/python/
```

💢 If the program is not installed, no output will appear.

---

### 2. Using `find` for advanced file searching

**Description:** We use `find` to search for specific files based on multiple criteria like type, name, size, date, and user.

```bash
find / -type f -name "*.conf" -user root -size +20k -newermt 2020-03-03 -exec ls -al {} \; 2>/dev/null
```

**Option Breakdown:**

| Function                                 | Option               |
| ---------------------------------------- | -------------------- |
| Search for files only                    | `-type f`            |
| Search for files ending with `.conf`     | `-name "*.conf"`     |
| Files owned by root                      | `-user root`         |
| File size greater than 20 KB             | `-size +20k`         |
| Modified after a specific date           | `-newermt 2020-03-03`|
| Execute `ls -al` on each result          | `-exec ls -al {} \;` |
| Suppress errors from protected files     | `2>/dev/null`        |

---

## 📊 Outcomes & Key Takeaways

* **Positive Result:** I successfully used `find` to filter system files precisely and located programs using `which`.  
* **Challenge Faced:** Handling errors from protected files, resolved using `2>/dev/null`.  
* **Core Lesson:** The power of `find` lies in its precise filtering, making it essential for investigations and system analysis.

---

## 🔗 Keywords & Resources

### 🏷️ Keywords / Tags  
`Linux`, `File_Search`, `which`, `find`, `CLI`, `System_Analysis`

### 📚 Further Reading  
1. [Linux Command Line Basics](https://linuxcommand.org/)  
2. [Exploring the find command](https://www.gnu.org/software/findutils/manual/html_node/find.html)

---
