# 🌿 Git Cheat Sheet

> 💡 **Emoji input**
>
> - **Windows:** `Win + .`
> - **macOS:** `Ctrl + Cmd + Space`

> 🌿 **Git quick help**
>
> - Show local branches: `git branch`
> - Show remote branches: `git branch -r`
> - Show all branches: `git branch -a`
> - Switch branch: `git checkout <branch>`
> - Create & switch branch: `git checkout -b <branch>`
> - Sync remote refs: `git fetch --all --prune`

---

## 🔧 Repository Setup

| Command | Description |
|-------|-------------|
| `git init` | Initialize a new repository |
| `git clone <url>` | Clone remote repository |
| `git remote -v` | Show remotes |
| `git remote add origin <url>` | Add remote origin |

---

## 📄 Status & Changes

| Command | Description |
|-------|-------------|
| `git status` | Show working tree status |
| `git diff` | Show unstaged changes |
| `git diff --staged` | Show staged changes |
| `git add <file>` | Stage file |
| `git add .` | Stage all changes |
| `git reset <file>` | Unstage file |

---

## 💾 Commit

| Command | Description |
|-------|-------------|
| `git commit -m "message"` | Create commit |
| `git commit --amend` | Amend last commit |
| `git log` | Commit history |
| `git log --oneline --graph` | Compact history |

---

## 🌿 Branching

| Command | Description |
|-------|-------------|
| `git branch` | List local branches |
| `git branch -r` | List remote branches |
| `git branch -a` | List all branches |
| `git branch -v` | Branch with last commit |
| `git branch -vv` | Branch with upstream |
| `git branch --show-current` | Show current branch |
| `git checkout <branch>` | Switch branch |
| `git checkout -b <branch>` | Create new branch |
| `git branch -d <branch>` | Delete local branch |
| `git branch -D <branch>` | Force delete branch |

---

## 🔀 Merge & Rebase

| Command | Description |
|-------|-------------|
| `git merge <branch>` | Merge branch |
| `git rebase <branch>` | Rebase branch |
| `git rebase -i HEAD~3` | Interactive rebase |
| `git abort --merge` | Abort merge |
| `git rebase --abort` | Abort rebase |

---

## 🌐 Remote & Sync

| Command | Description |
|-------|-------------|
| `git fetch` | Fetch remote changes |
| `git pull` | Fetch + merge |
| `git pull --rebase` | Fetch + rebase |
| `git push` | Push changes |
| `git push -u origin <branch>` | Push and set upstream |
| `git fetch --all --prune` | Sync and clean |

---

## 🧹 Cleanup & Maintenance

| Command | Description |
|-------|-------------|
| `git branch --merged` | List merged branches |
| `git branch --no-merged` | List unmerged branches |
| `git clean -fd` | Remove untracked files |
| `git gc` | Garbage collection |

⚠️ **Warning:** `git clean -fd` permanently deletes files!

---

## 🏷️ Tags & Releases

| Command | Description |
|-------|-------------|
| `git tag` | List tags |
| `git tag v1.0.0` | Create tag |
| `git push --tags` | Push tags |
| `git show v1.0.0` | Show tag details |

---

## 🔍 Troubleshooting

| Problem | Command |
|-------|---------|
| Wrong branch | `git checkout <branch>` |
| Reset to last commit | `git reset --hard HEAD` |
| Undo last commit | `git reset --soft HEAD~1` |
| Remove remote branch | `git push origin --delete <branch>` |
| Fix detached HEAD | `git checkout main` |

---

## 🧠 Best Practices

- Commit often, with clear messages
- Use feature branches
- Pull before push
- Avoid force push on shared branches
- Keep `main` always deployable


