
---

#  **Module 1: Git Setup and Configuration**  
##  **Lesson 1.1 – Installing Git**

---

###  **Objective:**
By the end of this lesson, learners will be able to:
- Install Git on **Windows**, **macOS**, and **Linux**
- Verify the installation and check the installed version
- Troubleshoot common installation issues

---

##  **Concepts First: What Does It Mean to 'Install Git'?**

Git is a **distributed version control system**, and like any tool, it must be installed on your machine to interact with your local files and repositories. Installing Git gives you access to:
- Git CLI (`git` command)
- Configuration and credential storage
- Git GUI tools (optional)
- Git Bash on Windows (Linux-like CLI)

---

##  **Step-by-Step: Installing Git**

---

###  **1. Installing Git on Windows**

####  Step-by-Step:
1. Go to the official website:  
    [https://git-scm.com](https://git-scm.com)
2. Click on the **Windows download link** (auto-detected).
3. Run the installer (`.exe` file).
4. During setup, **use default options**, but pay attention to:
   - **Choose the default editor** (use Notepad++ or VS Code if preferred).
   - **Select "Git from the command line and also from 3rd-party software"**.
   - Enable **Git Credential Manager**.
5. Complete the installation and launch **Git Bash** from the Start Menu.

####  Lab:
Open **Git Bash** and run:
```bash
git --version
```
 Expected Output: `git version 2.x.x`

---

###  **2. Installing Git on macOS**

####  Step-by-Step:
**Option 1: Using Xcode Command Line Tools**
```bash
xcode-select --install
```
(Installs Git along with developer tools)

**Option 2: Using Homebrew**
```bash
brew install git
```

####  Lab:
Verify installation:
```bash
git --version
```

---

###  **3. Installing Git on Linux**

####  Step-by-Step:
**Debian/Ubuntu:**
```bash
sudo apt update
sudo apt install git -y
```

**Red Hat/CentOS/Fedora:**
```bash
sudo dnf install git -y
```

**Arch Linux:**
```bash
sudo pacman -S git
```

####  Lab:
After installation:
```bash
git --version
```

---

##  **Troubleshooting & Common Issues**

| Problem | Reason | Solution |
|--------|--------|----------|
| `git: command not found` | PATH not set or Git not installed | Reinstall Git or restart terminal |
| Outdated version | Pre-installed Git version is too old | Manually install latest from [git-scm.com](https://git-scm.com) |
| Git GUI not available | GUI tools not installed | Use Git Bash or CLI |

---

##  Hands-on Lab Checklist

| Task | Status |
|------|--------|
| Installed Git on your OS  |  YES |
| Verified version using `git --version` |  YES  |
| Opened Git Bash or Terminal |  YES  |
| Explored where Git was installed (`which git`) |  YES  |

---

##  Pro Tip:
Use `where git` (Windows CMD) or `which git` (macOS/Linux) to see Git’s installation path.

---

##  Recap Summary

| Step | Windows | macOS | Linux |
|------|---------|--------|--------|
| Download Method | `.exe` from git-scm.com | `xcode-select` or `brew` | `apt`, `dnf`, or `pacman` |
| Verify | `git --version` | `git --version` | `git --version` |
| Tool Used | Git Bash | Terminal | Terminal |

---

