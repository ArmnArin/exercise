# 🔒 Docker Security

Security best practices for building and running Docker containers.

---

## 🚫 Avoid Running as Root

```dockerfile
USER 1000
```

```bash
docker run --user 1000:1000 myimage
```

---

## 🔐 Secrets Management

❌ Do NOT:
- store secrets in images
- commit secrets to Git

✅ Use:
- environment variables
- Docker secrets
- external secret managers

---

## 🧹 Minimal Images

```dockerfile
FROM node:20-alpine
```

Benefits:
- smaller size
- fewer vulnerabilities
- faster startup

---

## 📁 .dockerignore

```txt
node_modules
.git
.env
*.log
```

---

## 🔍 Image Scanning

```bash
docker scan myimage
```

or tools like:
- Trivy
- Snyk
- Grype

---

## 🌐 Network Isolation

- Use custom networks
- Avoid `--network=host`
- Expose only required ports

---

## 🧠 Best Practices

- Pin image versions
- Regularly rebuild images
- Use read-only volumes
- Limit container capabilities
- Keep Docker updated

---

## 📚 References

- https://docs.docker.com/engine/security/
