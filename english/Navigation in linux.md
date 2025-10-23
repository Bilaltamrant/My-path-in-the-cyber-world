
# 📚 Linux Navigation

**Date:** [October 23, 2025]  
**Level:** Beginner  
**Status:** 🟢 Completed

---

## 🎯 Goals / Objectives

* Learn how to navigate between directories in Linux using the terminal.
* Gain practical skills in listing contents, using shortcuts, and clearing the screen.

---

## 📝 Summary & Core Concepts

In this lesson, we explored the basic navigation commands in Linux, such as checking the current path, listing files, moving between directories, and using terminal shortcuts to speed up workflow. These skills form the foundation for any Linux user who wants to control the system via the command line.

### 📑 Key Concepts
* **pwd:** Displays the full path of the current directory.
* **ls:** Lists the contents of a directory.
* **cd:** Used to move between directories.
* **Terminal shortcuts:** Tools to speed up navigation, cleaning, and command history search.

---

## ⚙️ Practical Commands & Examples

### 1. Check your current location

**Description:** Shows the full path of the current working directory.

```bash
pwd
```

---

### 2. List directory contents

**Description:** Displays files and folders in the current path.

```bash
ls
```

---

### 3. Show detailed listing

**Description:** Displays additional info like permissions, owner, size, and date.

```bash
ls -l
```

---

### 4. Show hidden files

**Description:** Lists everything including hidden files that start with `.`.

```bash
ls -la
```

---

### 5. Navigate to a specific directory

**Description:** Move directly to a specified folder.

```bash
cd /var/log
```

---

### 6. Return to the previous directory

**Description:** Go back to the last visited directory.

```bash
cd -
```

---

### 7. Go to the home directory

**Description:** Navigate to the user's home folder.

```bash
cd ~
```

---

### 8. Move up one level

**Description:** Go to the parent directory of the current folder.

```bash
cd ..
```

---

### 9. Terminal Shortcuts

| Shortcut     | Function                            |
|--------------|-------------------------------------|
| `TAB`        | Auto-complete commands or paths     |
| `Ctrl + L`   | Clear the screen                    |
| `↑ / ↓`      | Navigate through command history    |
| `Ctrl + R`   | Search through command history      |

---

### 10. Full Example Scenario

**Description:** Execute a sequence of commands inside a sample directory.

```bash
# List all files inside /home/htb-student
ls -la

# Navigate to the network directory
cd /etc/network

# Return to the previous directory
cd -

# Clear the screen
clear
# or
Ctrl + L
```

---

## 📊 Outcomes & Key Takeaways

* **Positive Result:** Successfully navigated directories and understood system structure.
* **Challenge Faced:** Forgot some exact paths, solved using `TAB` for auto-completion.
* **Core Lesson:** The Linux terminal is powerful, and even simple commands can save a lot of time.

---

## 🔗 Keywords & Resources

### 🏷️ Keywords / Tags
`Linux`, `Navigation`, `Terminal`, `Bash`, `CLI`, `File_System`

### 📚 Further Reading
1. [Linux Command Line Basics](https://linuxcommand.org/)
2. [The Linux Command Line Book](https://linuxcommand.org/tlcl.php)
