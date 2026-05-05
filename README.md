## 👋 Welcome to ghost 🚀

Professional publishing platform and blogging CMS

## 📋 Description

Professional publishing platform and blogging CMS

## 🚀 Services

- **app**: ghost:latest

### Infrastructure Components

- **db**: Mysql database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/ghost/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/ghost" ~/.local/srv/docker/ghost
cd ~/.local/srv/docker/ghost
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install ghost
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
DB_ADMIN_NAME=root
DB_CREATE_DATABASE_NAME=ghost
DB_ADMIN_PASS=changeme_db_password
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:60190

## 📂 Volumes

- `./volumes/data/ghost` - Data storage
- `./volumes/data/db/mysql/ghost` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
