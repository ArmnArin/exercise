# 🛠️ Docker Troubleshooting

Common Docker problems and how to fix them.

---

## 🔁 Container Restarting

```bash
docker ps -a
docker logs <container_id>
```

Common causes:
- missing env variables
- wrong command
- permission issues

---

## 🚪 Port Already in Use

```bash
ss -tulpn | grep 8080
docker ps
```

Solution:
- stop conflicting service
- change exposed port

---

## 💾 Volume Permission Issues

```bash
ls -ln /path/to/volume
```

```bash
sudo chown -R 1000:1000 /path/to/volume
```

---

## 🧹 Disk Space Full

```bash
docker system df
docker system prune
```

⚠️ Removes unused resources

---

## 🌐 Network Issues

```bash
docker network ls
docker network inspect <network>
```

```bash
curl http://service:port
```

---

## 🧰 Debug Checklist

- Check logs
- Check ports
- Check permissions
- Check env vars
- Restart container

---

## 📚 References

- https://docs.docker.com/config/containers/troubleshoot/
