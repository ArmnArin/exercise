> 💡 **How to insert emojis like 🐧,📁,📄,etc. **
>
> - **Windows:** Press `Win + .`
> - **macOS:** Press `Ctrl + Cmd + Space`


# 🐧 Linux Command Cheat Sheet

A compact and structured overview of the most important Linux commands  
for system administration, DevOps, Docker, server operations, and troubleshooting.

---

## 📁 File System & Navigation

| Command | Description |
|-------|-------------|
| `pwd` | Show current working directory |
|   etc.   |      etc.    |


---

## 📄 Files & Content

| Command | Description |
|-------|-------------|
| `cat file` | Display file content |
|   etc.   |      etc.    |


---
## 🗂 File & Directory Management

| Command | Description |
|-------|-------------|
| `mkdir directory` | Create directory |
| `mkdir -p a/b/c` | Create nested directories |
|   etc.   |      etc.    |

⚠️ **Warning:** `rm -rf` is irreversible!

---
## 🔐 Permissions & Ownership

| Command | Description |
|-------|-------------|
|   etc.   |      etc.    |

**Permission logic:**  
`r = read (4)` · `w = write (2)` · `x = execute (1)`
---

## 🧠 Processes & System Status

| Command | Description |
|-------|-------------|
|   etc.   |      etc.    |

---

## 💾 Storage & Disk Usage

| Command | Description |
|-------|-------------|
| `df -h` | Disk usage |
|   etc.   |      etc.    |

---
## 🌐 Networking

| Command | Description |
|-------|-------------|
| `ip a` | Show network interfaces |
|   etc.   |      etc.    |

---

## 📦 Package Management (Debian/Ubuntu)

| Command | Description |
|-------|-------------|
| `apt update` | Update package list |
|   etc.   |      etc.    |

---

## 🐳 Docker (Essentials)

| Command | Description |
|-------|-------------|
| `docker ps` | List running containers |
|   etc.   |      etc.    |

---

## 📜 Logs & Debugging

| Command | Description |
|-------|-------------|
|   etc.   |      etc.    |


---

## 🔄 Archives & Compression

| Command | Description |
|-------|-------------|
|   etc.   |      etc.    |


## 🔑 SSH & Security

| Command | Description |
|-------|-------------|
| `ssh user@host` | SSH login |
|   etc.   |      etc.    |

---

## 🧪 Useful One-Liners

```bash
# Top 10 largest files
du -ah / | sort -rh | head -10

# Top memory-consuming processes
ps aux --sort=-%mem | head

# Top CPU-consuming processes
ps aux --sort=-%cpu | head

# Live free memory
watch free -h