
---

##  **0.3 Git vs GitHub vs GitLab vs Bitbucket**

Arjun’s development journey was going great. He finally understood Git, started using branches, committing regularly, and could roll back changes without panic.

But one day, his tech lead asked,  
> “Arjun, can you push your changes to **GitHub** and open a **pull request**?”

Arjun was confused.

> “Wait… I’m already using Git. Isn’t GitHub the same thing?”

---

###  Here’s Where Most Developers Get Confused

Let’s break it down in a **simple way**:

| Tool      | What It Is                             | Where It Works             |
|-----------|-----------------------------------------|----------------------------|
| **Git**   | A **tool** installed on your computer. A version control system to track changes locally. | On your **laptop or desktop** |
| **GitHub**| A **cloud platform** to host Git repositories. | On the **internet (cloud)**   |
| **GitLab**| Similar to GitHub, but built for CI/CD pipelines and enterprise DevOps workflows. | Cloud or self-hosted         |
| **Bitbucket**| Atlassian's Git-based platform, tightly integrated with Jira and Trello. | Cloud or self-hosted         |

---

###  Simple Analogy:
- **Git** is like using Microsoft Word on your laptop.
- **GitHub/GitLab/Bitbucket** are like Google Docs—where you can **store, collaborate, and share** that document with your team in real time.

---

###  Real-World Dev Workflow with Git & GitHub

Arjun’s team follows this Git + GitHub workflow:

1. **Clone** the repo from GitHub to his laptop.
2. Create a **new branch**: `feature/payment-method`.
3. Code and commit regularly using Git.
4. **Push** the branch to GitHub.
5. Raise a **Pull Request** for code review.
6. Teammates review and comment.
7. After approval, it's **merged into main** and automatically deployed via CI/CD.

 Now the whole team is in sync.  
 Every change is reviewed, tested, and traceable.  
 GitHub acts as the **source of truth** for the project.

---

###  GitHub vs GitLab vs Bitbucket – What to Choose?

| Feature               | GitHub                       | GitLab                           | Bitbucket                      |
|-----------------------|------------------------------|----------------------------------|-------------------------------|
| Best For              | Open Source & Community      | DevOps & Internal Enterprise CI  | Jira/Trello-based Workflows   |
| CI/CD Support         | GitHub Actions               | Built-in GitLab CI               | Bitbucket Pipelines           |
| Free Private Repos    | Yes                          | Yes                              | Yes                           |
| Self-Hosting Option   | No (cloud only)              | Yes (self-hosted GitLab CE/EE)   | Yes (Bitbucket Server)        |
| Used By               | Microsoft, Facebook, Netflix | CERN, NASA, Alibaba              | Teams using Atlassian Suite   |

---

###  Real Use Case:
Arjun’s startup works with GitHub because they build open-source tools.  
His friend Priya works in an enterprise setup where everything is self-hosted—so they use **GitLab** with built-in CI/CD.  
Kabir works in a product-based company using **Jira**—so their team prefers **Bitbucket** for seamless integration.

Each has its place. **You use Git everywhere**, but you choose a hosting platform based on your team’s workflow.

---

###  Key Takeaways:
- **Git** is the engine.  
- **GitHub/GitLab/Bitbucket** are the dashboard + garage + community.
- You **commit and manage code with Git**, and **collaborate, review, and deploy using GitHub-like platforms**.

---

