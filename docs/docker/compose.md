# 🧩 Docker Compose

Docker Compose is used to define and run **multi-container applications** using a single YAML file.

---

## 📦 What is Docker Compose?

Docker Compose allows you to:
- run multiple services together
- define networks and volumes
- manage environments consistently
- start/stop everything with one command

---

## ▶️ Basic Commands

```bash
docker compose up
docker compose up -d
docker compose down
docker compose restart
docker compose ps
docker compose logs
docker compose logs -f
```

---

## 📄 Minimal docker-compose.yml

```yml
version: "3.9"

services:
  web:
    image: nginx
    ports:
      - "8080:80"
```

---

## 🧱 Multi-Service Example

```yml
version: "3.9"

services:
  app:
    image: myapp:latest
    depends_on:
      - db
    environment:
      DB_HOST: db

  db:
    image: postgres:15
    environment:
      POSTGRES_DB: appdb
      POSTGRES_USER: appuser
      POSTGRES_PASSWORD: secret
    volumes:
      - db-data:/var/lib/postgresql/data

volumes:
  db-data:
```

---

## 🌐 Networks

```yml
networks:
  backend:
```

```yml
services:
  app:
    networks:
      - backend
```

---

## 💾 Volumes

```yml
volumes:
  app-data:
```

```yml
services:
  app:
    volumes:
      - app-data:/data
```

---

## 🧠 Best Practices

- Use `.env` files
- Do not hardcode secrets
- Use `depends_on`
- Name services clearly
- Separate prod/dev files

---

## 📚 References

- https://docs.docker.com/compose/
