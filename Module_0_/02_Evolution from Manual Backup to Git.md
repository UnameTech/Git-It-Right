
---

##  **0.2 Evolution from Manual Backup to Git**

Let’s go back to Arjun.

After his lunch-break disaster, Arjun decided to never trust himself with just "Ctrl+S" again. He started **manually creating backups** every few hours.

His folder started looking like this:

```
transaction_v1.py  
transaction_v1_final.py  
transaction_v1_final_fixed.py  
transaction_final_latest_real.py  
```

But even this system had problems:
- He **couldn’t remember** which file had the actual working logic.
- If he deleted or overwrote something by mistake, there was **no way to track** what changed.
- If a teammate edited his file, **merging changes was a nightmare**.

It was still chaos—just better-organized chaos.

---

###  Enter: Version Control Systems

To solve this mess, the industry started developing **Version Control Systems (VCS)**.

There were two major types:

---

###  **1. Centralized Version Control (e.g., SVN, CVS)**

These systems had a **single central server** that stored all project files and history. Developers had to **check out** files, make changes, and **check them back in**.

####  How it worked:
- Arjun connects to the central server and checks out `transaction.py`.
- No one else can edit the file while he has it checked out.
- After editing, he checks it back in.
  
This **prevented overwrites**, but had its flaws:
- No offline access—Arjun **couldn’t work on a flight**.
- If the central server went down, **work stopped** for everyone.
- Branching was difficult and slow.

---

### 🔸 **2. Distributed Version Control (e.g., Git, Mercurial)**

Then came **Git**—a **revolutionary tool** created by Linus Torvalds in 2005 for Linux kernel development.

In Git, **every developer has a full copy of the codebase, including its history**. You can commit, branch, diff, and revert entirely **offline**.

####  Arjun's new life with Git:
- At **9:00 AM**, he creates a **new branch** for a feature.
- At **2:00 PM**, he commits his changes.
- Even if his system crashes, he can clone the project from GitHub and be up and running in minutes.
- He can collaborate with his team using **branches and pull requests**, without stepping on anyone's toes.

---

###  Comparison Table

| Feature                         | Manual Backup | SVN (Centralized VCS) | Git (Distributed VCS) |
|-------------------------------|---------------|------------------------|------------------------|
| Collaboration Support          |  No          |  Limited              |  Full                |
| Offline Work                   |  No          |  No                   |  Yes                 |
| History & Change Tracking      |  Manual      |  Yes                  |  Advanced            |
| Branching & Experimentation    |  Not Possible|  Difficult            |  Fast & Easy         |
| Rollback to Working State      |  No          |  To a point           |  Robust              |
| Disaster Recovery              |  None        |  Server-dependent     |  Local + Remote      |

---

###  Real-World Scenario: Team Collaboration

Let’s say Arjun, Priya, and Kabir are all working on the same project.

- **Without Git**: They email files or upload them to shared drives, ending up with multiple confusing copies.
- **With Git**: Each developer creates a **branch**, works independently, and raises a **pull request**. Git tracks every change and helps **merge their work safely**.

---

By switching to Git, Arjun doesn’t just **save his code**—he saves time, avoids bugs, improves teamwork, and becomes a more **confident developer**.

---

Up next:  
 **0.3 Git vs GitHub vs GitLab vs Bitbucket**  
