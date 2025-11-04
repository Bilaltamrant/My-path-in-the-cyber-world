
# 📚 File Descriptors and Redirection in Linux

**Date:** Tuesday, November 4, 2025  
**Level:** Intermediate  
**Status:** 🟢 Completed

---

## 🎯 Goals / Objectives

- Understand the concept of File Descriptor (FD) in Linux.  
- Learn how to use redirection and pipes to control input and output.

---

## 📝 Summary & Core Concepts

In Linux, every file or input/output operation is represented by a number called a **File Descriptor (FD)**.  
The kernel uses this number to track open files for each process.  
Think of it like a ticket system:  
- Ticket = FD number  
- Person = file  
- Clerk = operating system  

### 📑 Key Concepts
- **File Descriptor (FD):** A unique number for each file or I/O stream.  
- **STDIN / STDOUT / STDERR:** Standard input/output/error descriptors in Linux.

---

## ⚙️ Practical Commands & Examples

### 1. The Three Standard Descriptors in Linux

| Function                                | Number | Name     |
| -------------------------------------- | ------ | -------- |
| Standard input (e.g., keyboard)         | 0      | `STDIN`  |
| Standard output (e.g., results)         | 1      | `STDOUT` |
| Standard error (e.g., warnings/errors)  | 2      | `STDERR` |

---

### 2. Examples Using FD

#### Example with `cat`

```bash
cat
```

- Waits for user input via FD 0  
- Displays input directly via FD 1  
- Example: You type "ssd" → it echoes "ssd"

---

#### Example with `find`

```bash
find /etc/ -name shadow
```

- If the file is found → output via FD 1  
- If access is denied → error via FD 2

---

### 3. Redirection

#### Redirecting Errors to `/dev/null`

```bash
find /etc/ -name shadow 2>/dev/null
```

- `2>` means redirect FD 2  
- `/dev/null` is a dummy device that discards data

---

#### Redirecting Output to a File

```bash
find /etc/ -name shadow 2>/dev/null > result.txt
```

- `>` means redirect FD 1 to a file

---

#### Redirecting `STDOUT` and `STDERR` Separately

```bash
find /etc/ -name shadow 2> stdt.txt 1> smd.txt
```

- Errors → `stdt.txt`  
- Output → `smd.txt`

---

#### Redirecting `STDIN` from a File

```bash
cat < result.txt
```

- Input comes from the file instead of the keyboard

---

#### Appending `STDOUT` to a File

```bash
find /etc/ -name passwd >> result.txt 2>/dev/null
```

- `>>` appends results without overwriting existing content

---

#### Multi-line Input Using `EOF`

```bash
cat << EOF > result.txt
```

- Opens manual input until `EOF` is typed  
- `EOF` here means "End Of File" — not written into the file

---

### 4. Using Pipes `|`

- Connects two commands: output of the first → input of the second

```bash
ls /etc | grep passwd
```

- `ls` lists files  
- `grep` filters results containing "passwd"

---

#### Important Notes

- Pipes transfer `STDOUT` only  
- To include errors:

```bash
command 2>&1 | command
```

---

## 📊 Outcomes & Key Takeaways

- **Positive Result:** Learned how to control data flow using FD and redirection.  
- **Challenge Faced:** Differentiating between `STDOUT` and `STDERR` in complex commands.  
- **Key Lesson:** Redirection and pipes are powerful tools for organizing output and analyzing results.

---

## 🔗 Keywords & Resources

### 🏷️ Keywords / Tags

`Linux`, `File_Descriptor`, `STDIN`, `STDOUT`, `STDERR`, `Redirection`, `Pipes`, `Shell`

### 📚 Further Reading

1. [Linux File Descriptors Explained](https://linuxize.com/post/file-descriptors-in-linux/)  
2. [Redirection in Bash](https://tldp.org/LDP/abs/html/io-redirection.html)  
3. [Advanced Bash Scripting Guide](https://tldp.org/LDP/abs/html/)
```
