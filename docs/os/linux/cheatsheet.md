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
| `ls` | List files and directories |
| `ls -lah` | Detailed list including hidden files |
| `cd /path` | Change directory |
| `cd ..` | Go one level up |
| `tree` | Display directory structure as a tree |
| `stat file` | Show detailed file information |

---

## 📄 Files & Content

| Command | Description |
|-------|-------------|
| `cat file` | Display file content |
| `less file` | View file page by page |
| `head -n 20 file` | Show first 20 lines |
| `tail -n 20 file` | Show last 20 lines |
| `tail -f logfile.log` | Follow log file in real time |
| `wc -l file` | Count number of lines |
| `file file` | Detect file type |

---

## 🗂 File & Directory Management

| Command | Description |
|-------|-------------|
| `mkdir directory` | Create directory |
| `mkdir -p a/b/c` | Create nested directories |
| `rm file` | Delete file |
| `rm -rf directory` | Recursively delete directory |
| `cp source target` | Copy file |
| `cp -r source target` | Copy directory |
| `mv old new` | Rename or move |

⚠️ **Warning:** `rm -rf` is irreversible!

---

## 🔐 Permissions & Ownership

| Command | Description |
|-------|-------------|
| `ls -l` | Show permissions |
| `chmod 755 file` | Set permissions |
| `chmod -R 750 directory` | Set permissions recursively |
| `chown user:group file` | Change ownership |
| `id user` | Show UID / GID |

**Permission logic:**  
`r = read (4)` · `w = write (2)` · `x = execute (1)`

---

## 🧠 Processes & System Status

| Command | Description |
|-------|-------------|
| `ps aux` | Show all running processes |
| `top` | Live process overview |
| `htop` | Enhanced process viewer (if installed) |
| `uptime` | System uptime and load |
| `free -h` | Memory usage |
| `vmstat` | Memory and CPU statistics |
| `watch -n 1 command` | Run command repeatedly |

---

## 💾 Storage & Disk Usage

| Command | Description |
|-------|-------------|
| `df -h` | Disk usage |
| `du -sh directory` | Directory size |
| `lsblk` | List block devices |
| `mount` | Show mount points |
| `find /path -size +1G` | Find large files |

---

## 🌐 Networking

| Command | Description |
|-------|-------------|
| `ip a` | Show network interfaces |
| `ip r` | Show routing table |
| `ss -tulpen` | List open ports |
| `ping host` | Test connectivity |
| `curl url` | HTTP request |
| `wget url` | Download file |
| `nc -zv host port` | Test port connectivity |

---

## 📦 Package Management (Debian/Ubuntu)

| Command | Description |
|-------|-------------|
| `apt update` | Update package list |
| `apt upgrade` | Install updates |
| `apt install package` | Install package |
| `apt remove package` | Remove package |
| `apt purge package` | Remove package including config |
| `dpkg -l` | List installed packages |

---

## 🐳 Docker (Essentials)

| Command | Description |
|-------|-------------|
| `docker ps` | List running containers |
| `docker ps -a` | List all containers |
| `docker images` | List images |
| `docker logs container` | Show container logs |
| `docker exec -it c bash` | Enter container shell |
| `docker stop c` | Stop container |
| `docker rm c` | Remove container |
| `docker-compose up -d` | Start stack |
| `docker-compose down` | Stop stack |

---

## 📜 Logs & Debugging

| Command | Description |
|-------|-------------|
| `journalctl -xe` | Systemd logs |
| `journalctl -u service` | Service logs |
| `dmesg` | Kernel messages |
| `strace cmd` | Debug system calls |
| `lsof -i :443` | Check which process uses port 443 |

---

## 🔄 Archives & Compression

| Command | Description |
|-------|-------------|
| `tar -czvf a.tar.gz directory` | Create archive |
| `tar -xzvf a.tar.gz` | Extract archive |
| `zip -r a.zip directory` | Create ZIP archive |
| `unzip a.zip` | Extract ZIP archive |

---

## 🔑 SSH & Security

| Command | Description |
|-------|-------------|
| `ssh user@host` | SSH login |
| `ssh -i key user@host` | SSH using key |
| `scp file user@host:/path` | Copy file over SSH |
| `chmod 600 key.pem` | Secure SSH key |
| `fail2ban-client status` | Fail2Ban status |

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
