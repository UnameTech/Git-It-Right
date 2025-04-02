
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

