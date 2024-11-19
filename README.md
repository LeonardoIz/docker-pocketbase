# Docker PocketBase
A Docker image for PocketBase

### How to use?
* **Docker Run:**
```
docker run -d \
  --name pocketbase \
  -p 8080:8080 \
  --restart unless-stopped \
  ghcr.io/leonardoiz/pocketbase:latest

```

* **Docker Compose**
```
version: '3.8'

services:
  pocketbase:
    image: ghcr.io/leonardoiz/pocketbase:latest
    container_name: pocketbase
    ports:
      - 8080:8080
    restart: unless-stopped
```