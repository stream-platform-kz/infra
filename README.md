# Stream Platform - Infra

This repository contains the **infrastructure stack** for the Stream Platform project.  
It provides databases, message brokers, storage, and media servers needed by the backend microservices.

---

## 🚀 Stack

Services included in `docker-compose.yml`:

- **PostgreSQL** → primary relational database
- **Redis** → caching & session store
- **Kafka + Zookeeper** → message broker for events
- **MinIO** → S3-compatible object storage (media uploads, files)
- **MediaMTX** → media server for handling RTMP/HLS streams

---

## 📦 Requirements

- [Docker Desktop](https://www.docker.com/products/docker-desktop) (macOS/Windows)
- [Docker Compose](https://docs.docker.com/compose/) (bundled with Docker Desktop)

---

## 🔧 Usage

### Start the stack
```bash
docker compose up -d