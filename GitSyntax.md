
- **Working Directory**: Your files on disk
- **Staging Area**: Prepared files for commit
- **Local Repository**: Commits stored locally
- **Remote Repository**: Shared repository (GitHub, GitLab, etc.)

---

## 🔧 Repository Setup

| Command | Description |
|-------|-------------|
| `git init` | Create a new Git repository |
| `git clone <HTTPS/SSH>` | Create a local copy of a remote repository |
| `git remote` | List remote repositories |
| `git remote -v` | Show remote URLs |

---

## 📄 Status & File Tracking

| Command | Description |
|-------|-------------|
| `git status` | Show current state of files |
| `git add <file>` | Add file to staging area |
| `git add .` | Add all files to staging area |
| `git rm --cached <file>` | Unstage file (stage → working directory) |
| `git diff` | Show file changes |
| `git diff --help` | Show diff help |

---

## 💾 Commit

| Command | Description |
|-------|-------------|
| `git commit -m "msg"` | Commit staged files |
| `git commit -a -m "msg"` | Stage tracked files and commit |
| ⚠️ | New files must be added once with `git add` |

---

## 📜 Commit History

| Command | Description |
|-------|-------------|
| `git log` | Show full commit history |
| `git log --help` | Log command help |
| `git log --oneline` | One commit per line |
| `git log -2 --oneline` | Last two commits |
| `git log -p` | Commits with file changes |
| `git log --graph` | Commit tree with branches |

---

## 🔄 Undo & Reset

| Command | Description |
|-------|-------------|
| `git checkout -- <file>` | Restore file to last commit |
| `git reset HEAD .` | Unstage all files |
| `git reset <commit>` | Soft reset (keep files) |
| `git reset --hard <commit>` | Hard reset (delete changes) |

⚠️ **Warning:** `--hard` deletes files permanently

---

## 🌐 Remote Sync

| Command | Description |
|-------|-------------|
| `git push <repository>` | Push local commits to remote |
| `git pull <repository>` | Update local branch from remote |

---

## 🌿 Branching

| Command | Description |
|-------|-------------|
| `git branch <name>` | Create branch |
| `git branch -l` | List local branches |
| `git branch -r` | List remote branches |
| `git branch -a` | List all branches |
| `git branch -d <name>` | Delete branch |
| `git switch <branch>` | Switch branch |
| `git checkout <branch>` | Switch branch |
| `git switch -c <branch>` | Create and switch |
| `git checkout -b <branch>` | Create and switch |

> ℹ️ Always check `git status` before switching branches.

---

## 🔀 Merge

| Command | Description |
|-------|-------------|
| `git merge <branch>` | Merge branch into current branch |

---

## 📦 Stash (Temporary Storage)

| Command | Description |
|-------|-------------|
| `git stash` | Save changes temporarily |
| `git stash save "msg"` | Save with message |
| `git stash push -m "msg"` | Save with message |
| `git stash list` | List stashes |
| `git stash show stash@{n}` | Show stash summary |
| `git stash show -p stash@{n}` | Show stash details |
| `git stash drop stash@{n}` | Delete stash |
| `git stash pop stash@{n}` | Apply and delete stash |
| `git stash apply stash@{n}` | Apply and keep stash |

---

## ⚙️ Configuration

| Command | Description |
|-------|-------------|
| `git config --global user.name "name"` | Set global username |
| `git config --global user.email "email"` | Set global email |
| `touch .gitignore` | Create .gitignore file |

---

## 🌍 GitHub Concepts

- **Fork**: A personal copy of another user's repository
- **Pull Request (PR)**: Request to merge changes into another branch/repository

---

## ✅ Best Practices

- Commit small and often
- Use feature branches
- Pull before push
- Never force-push to shared branches
- Keep `main` stable

---

📌 **Purpose:** Learning · Daily work · Team workflows  
📌 **Format:** GitHub / GitLab ready Markdown
