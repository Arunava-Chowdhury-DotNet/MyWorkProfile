# MyWorkProfile
This is my profile created using HTML. Updated from VS Code

# 🧾 Git vs GitHub CLI (gh) - Command Cheat Sheet

A quick comparison of essential commands using `git` (version control) and `gh` (GitHub CLI).

---

## 📦 Common Commands

| **Purpose**                | `git` Command                              | `gh` Command                                  |
|----------------------------|---------------------------------------------|-----------------------------------------------|
| ✅ Initialize a repo       | `git init`                                  | –                                             |
| 🧬 Clone a repo            | `git clone https://github.com/user/repo.git`| `gh repo clone owner/repo`                    |
| ➕ Stage changes           | `git add filename`                          | –                                             |
| 💾 Commit changes         | `git commit -m "Message"`                   | –                                             |
| 🔄 Push to GitHub         | `git push origin branch-name`               | –                                             |
| ⬇️ Pull changes           | `git pull origin branch-name`               | –                                             |
| 🌿 Create a branch         | `git checkout -b new-branch`                | –                                             |
| 🔁 Merge branches         | `git merge other-branch`                    | –                                             |
| 🚀 View repo in browser   | –                                           | `gh repo view --web`                          |
| 🍴 Fork a repo            | –                                           | `gh repo fork`                                |
| 🧪 Create a Pull Request  | –                                           | `gh pr create --base main --head my-branch`   |
| 📋 List issues            | –                                           | `gh issue list`                               |
| 🔐 Authenticate GitHub    | –                                           | `gh auth login`                               |
| 🔑 Add SSH key to GitHub  | –                                           | `gh ssh-key add ~/.ssh/id_ed25519.pub`        |

---

## ✅ Example Workflow Using Both

```bash
# 1. Clone your fork
gh repo clone your-username/repo-name
cd repo-name

# 2. Create a new branch
git checkout -b feature-xyz

# 3. Make changes, then add & commit
git add .
git commit -m "Added feature XYZ"

# 4. Push branch to GitHub
git push -u origin feature-xyz

# 5. Create a Pull Request
gh pr create --base main --head feature-xyz --fill
