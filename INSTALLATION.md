# Installation Guide

This guide covers all installation methods for Live AI.

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

## Operating System Installation

### macOS Installation

1. Download and extract the ZIP file
2. Open Terminal and navigate to the extracted folder
3. Run: `./live-ai`

**Note**: The binaries are signed and notarized by the developer for security.

### Linux Installation

1. Download and extract the ZIP file
2. Open Terminal and navigate to the extracted folder
3. Run: `./live-ai`

**Note**: Make sure the file has execution permissions. If needed, run: `chmod +x live-ai`

### Windows Installation

1. Download and extract the ZIP file
2. Double-click on `live-ai.exe` or run from Command Prompt

## Available Versions

In the [Releases](https://github.com/mosqueiro/live-ai/releases) section you'll find 3 executable versions:

- **macOS**: Executable binary for macOS
- **Linux**: Executable binary for Linux
- **Windows**: `.exe` executable for Windows

**Docker Version**: Available in the repository via `docker-compose.yml` file (Recommended)

The Docker version is most recommended as it offers complete isolation and automatic configuration of persistent volumes.

## Downloads

Executable files are available in the [Releases](https://github.com/mosqueiro/live-ai/releases) section for direct download.

## Next Steps

After installation, proceed to:

1. [Getting Your Free API Key](GETTING_API_KEY.md) - Obtain your API key
2. [YouTube Live Setup](YOUTUBE_LIVE.md) - Configure your YouTube live stream
3. [Configuration](CONFIGURATION.md) - Configure the system settings
