# 📚 Editing Files in Linux Using nano and vim Editors

**Date:** [Creation Date]  
**Level:** Beginner  
**Status:** ✅ Complete

---

## 🎯 Goals / Objectives

* Learn about terminal text editors: nano and vim
* Learn basic usage of nano editor
* Understand vim modes and essential commands

---

## 📝 Summary & Core Concepts

In Linux, text files are used for everything: system settings, scripts, commands... To edit them, we need a terminal editor. The two most famous terminal text editors are:

- **nano**: Easy and simple, suitable for beginners.
- **vim**: Powerful and professional editor, requires some training.

### 📑 Key Concepts
* **Text Editor**: A program used to create and modify text files.
* **vim Modes**: Different editor states (Insert mode, Normal mode, Command mode) each with its own uses.

---

## ⚙️ Practical Commands & Examples

### 1. Using `nano` Editor

**Description:** Easy-to-use text editor for beginners.

```bash
# Open a new or existing file
nano filename.txt
```

**Basic nano shortcuts:**

| Function                  | Shortcut    |
| ------------------------- | ----------- |
| Save file                 | `ctrl + O`  |
| Exit editor               | `ctrl + X`  |
| Search in text            | `ctrl + W`  |
| Cut line                  | `ctrl + K`  |
| Paste line                | `ctrl + U`  |
| Insert another file       | `ctrl + R`  |

**Note:** When pressing `ctrl + W` and typing a word, the cursor moves to the first match. When pressing it again + `ENTER`, it moves to the next match.

### 2. Using `Vim` Editor

**Description:** Powerful multi-mode text editor.

```bash
# Open file in vim
vim filename.txt
```

#### Vim Editor Modes

| Mode      | Function                                           |
|-----------|----------------------------------------------------|
| Normal    | Execute commands like delete, copy, navigate       |
| Insert    | Insert text ← enter with `i`                       |
| Visual    | Select text ← enter with `v`                       |
| Command   | Execute commands like `:w`, `:q`, `:x`             |
| Replace   | Replace character with character ← enter with `R`  |
| Ex        | Execute advanced commands ← like `:g`, `:s`        |

#### Most Important Vim Commands

| Command      | Function                                 |
|--------------|------------------------------------------|
| `i`          | Enter insert mode                        |
| `:w`         | Save file                                |
| `:q`         | Exit editor                              |
| `:wq`        | Save and exit                            |
| `:x`         | Save and exit (same as `:wq`)            |
| `:help`      | Open help                                |
| `:Tutor`     | Open Vim training mode                   |
| `vimtutor`   | Open training mode from terminal         |

---

## 📊 Outcomes & Key Takeaways

* **Positive Outcome:** Successfully edited text files in terminal using both nano and vim editors efficiently.
* **Challenge Faced:** Getting used to different vim modes and saving/exiting using commands.
* **Key Lesson:** Understanding vim modes is the key to fully utilizing this powerful editor.

---

## 🔗 Keywords & Resources

### 🏷️ Keywords / Tags
`Linux`, `Text_Editors`, `nano`, `vim`, `CLI`, `File_Editing`, `Bash`, `Terminal`, `Command_Line`

### 📚 Further Reading
1. [Vim Official Documentation](https://www.vim.org/docs.php) - Official Vim Documentation
2. [GNU nano Documentation](https://www.nano-editor.org/dist/latest/nano.html) - nano Editor Documentation
3. [Vim Adventures](https://vim-adventures.com/) - Game for Learning Vim Commands
4. [Interactive Vim Tutorial](https://www.openvim.com/) - Interactive Vim Learning Tutorial
