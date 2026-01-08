---
title: Installation
order: 1
---

# Installation

This guide covers different ways to install NavHub.

## Docker (Recommended)

The easiest way to run NavHub is with Docker:

```bash
# Create a directory for NavHub
mkdir navhub && cd navhub

# Download docker-compose.yml
curl -O https://raw.githubusercontent.com/anthropics/navhub/main/docker-compose.yml

# Start the services
docker-compose up -d
```

### Environment Variables

Create a `.env` file to customize your installation:

```env
# Database
POSTGRES_USER=navhub
POSTGRES_PASSWORD=your-secure-password
POSTGRES_DB=navhub

# App
APP_SECRET=your-secret-key
APP_URL=http://localhost:8080
```

## Manual Installation

### Prerequisites

- Go 1.21 or later
- Node.js 18 or later
- PostgreSQL 13 or later
- Redis 6 or later (optional, for caching)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/anthropics/navhub.git
   cd navhub
   ```

2. **Install Go dependencies**
   ```bash
   go mod tidy
   ```

3. **Install frontend dependencies**
   ```bash
   cd frontend && npm install
   ```

4. **Configure the database**
   ```bash
   cp config/app.ini.example config/app.ini
   # Edit config/app.ini with your database settings
   ```

5. **Build and run**
   ```bash
   make build
   ./bin/navhub
   ```

## Verifying Installation

After installation, visit `http://localhost:8080`. You should see the NavHub login page.

## Troubleshooting

### Database Connection Error

Make sure PostgreSQL is running and the credentials in `config/app.ini` are correct.

### Port Already in Use

Change the port in `config/app.ini` or stop the conflicting service.
