# Installation Guide

This guide covers all installation methods for Live AI.

## Navigation

- [← Back to README](README.md)
- [🔑 Getting Your Free API Key](GETTING_API_KEY.md)
- [🎥 YouTube Live Setup](YOUTUBE_LIVE.md)
- [⚙️ Configuration](CONFIGURATION.md)
- [🔧 Troubleshooting](TROUBLESHOOTING.md)

## Docker Installation (Recommended)

### Prerequisites

- Docker and Docker Compose installed

### Running

1. Clone the repository:

```bash
git clone https://github.com/mosqueiro/live-ai.git
cd live-ai
```

2. Run with Docker Compose:

```bash
docker-compose up -d
```

The service will be available at `http://localhost:8080`

### ⚠️ **VERY IMPORTANT: Persistent Volumes**

**⚠️ WARNING: If you don't configure persistent volumes, ALL your data will be lost when the container is restarted!**

Application data is saved in the host's `./data` folder, mapped to `/app/data` in the container, ensuring your settings are maintained even after restarts.

**Why it's crucial:**

- Without persistent volumes, your YouTube settings will be lost
- Your streaming data and history will be erased
- You'll need to reconfigure everything again after each restart

## Docker Installation Only

Live AI is now available exclusively via Docker for the best experience and security.

## Next Steps

After installation, proceed to:

1. [Getting Your Free API Key](GETTING_API_KEY.md) - Obtain your API key
2. [YouTube Live Setup](YOUTUBE_LIVE.md) - Configure your YouTube live stream
3. [Configuration](CONFIGURATION.md) - Configure the system settings
