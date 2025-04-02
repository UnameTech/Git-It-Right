
---

#  **First-Time Git Setup (Global Configuration)**

---

##  Step 1: Install Git (Skip if already installed)

### For Ubuntu/Debian:
```bash
sudo apt update
sudo apt install git
```

---

##  Step 2: Check if Git is Installed
```bash
git --version
```
 Example Output:
```
git version 2.39.2
```

---

##  Step 3: Set Your Global Identity

###  Set your Git username:
```bash
git config --global user.name "Kumar"
```

###  Set your Git email:
```bash
git config --global user.email "kumar@example.com"
```

This info will appear in every commit you make from this system.

---

##  Step 4: Set Your Preferred Editor (Optional)

Example with nano:
```bash
git config --global core.editor "nano"
```

Other choices:
- Vim: `"vim"`
- VSCode: `"code --wait"`

---

##  Step 5: Set Default Branch Name to `main` (Recommended)

```bash
git config --global init.defaultBranch main
```

GitHub and many cloud providers use `main` by default now.

---

##  Step 6: View All Current Git Global Settings

```bash
git config --global --list
```

 Sample Output:
```
user.name=Kumar
user.email=kumar@example.com
core.editor=nano
init.defaultBranch=main
```

---

##  Step 7: Check the Config File (Optional)

Your global config is saved at:
```bash
~/.gitconfig
```

View it with:
```bash
cat ~/.gitconfig
```

---

##  Optional: Credential Helper (To Avoid Repeated Password Prompts)

### For temporary caching (15 min by default):
```bash
git config --global credential.helper cache
```

### For persistent (saved to disk):
```bash
git config --global credential.helper store
```

---

##  Quick Summary of Commands

```bash
git config --global user.name "Kumar"
git config --global user.email "kumar@example.com"
git config --global core.editor "nano"
git config --global init.defaultBranch main
git config --global --list
```

---
---


## **`.gitconfig` file**
---

#  `.gitconfig` in Git – Concept & Use Cases

---

##  What is `.gitconfig`?

The `.gitconfig` file is a **Git configuration file** used to store Git’s settings.

It defines:
- **Who you are** (user.name & user.email)
- **What your Git preferences are** (editor, merge tools, color settings, etc.)
- **Behavioral customizations** (aliases, credential caching, etc.)

---

##  Where is `.gitconfig` Stored?

Git supports **three levels of configuration**, and each has its own config file:

| Level         | Scope             | File Location                  |
|---------------|-------------------|--------------------------------|
| **System**     | All users, system-wide | `/etc/gitconfig`                |
| **Global**     | Specific user     | `~/.gitconfig` (or `%USERPROFILE%\.gitconfig` on Windows) |
| **Local**      | Specific project/repo | `project_folder/.git/config`   |

>  Local overrides Global, and Global overrides System settings.

---

##  How to View `.gitconfig`

```bash
cat ~/.gitconfig
```

Sample Output:
```ini
[user]
    name = Kumar
    email = kumar@example.com
[core]
    editor = nano
[init]
    defaultBranch = main
```

---

##  Sample `.gitconfig` File (Global)

```ini
[user]
    name = Kumar
    email = kumar@example.com

[core]
    editor = code --wait
    autocrlf = input

[alias]
    st = status
    co = checkout
    br = branch
    ci = commit

[color]
    ui = auto

[credential]
    helper = store
```

---

##  Use Cases of `.gitconfig`

### 🔹 1. **Identity Management**
Set your global name and email for all Git commits:
```ini
[user]
    name = Kumar
    email = kumar@example.com
```

---

###  2. **Custom Command Aliases**
Speed up daily work:
```ini
[alias]
    co = checkout
    br = branch
    ci = commit
    st = status
```
Usage:
```bash
git co -b new-feature   # git checkout -b new-feature
```

---

###  3. **Default Editor**
Choose your preferred text editor:
```ini
[core]
    editor = code --wait
```

---

###  4. **Branch Naming**
Set `main` as default branch instead of `master`:
```ini
[init]
    defaultBranch = main
```

---

###  5. **Credential Storage**
Remember GitHub/remote passwords:
```ini
[credential]
    helper = store
```

Or:
```ini
[credential]
    helper = cache
```

---

###  6. **Color Coding Git Output**
Improve CLI readability:
```ini
[color]
    ui = auto
```

---

###  7. **Platform Line Ending Control**
If you’re on Windows, avoid CRLF issues:
```ini
[core]
    autocrlf = true
```

---

##  BONUS: Open or Edit `.gitconfig` Easily

```bash
git config --global --edit
```

It opens the file in your default editor.

---

##  Summary

| Feature | Purpose |
|--------|---------|
| `.gitconfig` | Stores user-level Git settings |
| Used for | Name, email, aliases, editor, defaults |
| Location | `~/.gitconfig` (Global), `./.git/config` (Local) |
| Editable via | `git config` CLI or manually in file |

---


