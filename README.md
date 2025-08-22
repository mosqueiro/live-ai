# Live AI - Intelligent YouTube Streaming

Live AI is an innovative YouTube streaming software that uses artificial intelligence to automate and optimize your live streams.

**🔑 Get your API key at: [https://live.1click.ai/](https://live.1click.ai/)**

## Features

- 🤖 **AI Integration**: Uses artificial intelligence to improve streaming quality
- 📹 **Automatic Streaming**: Automated streaming to YouTube
- 💾 **Persistent Data**: Settings and data automatically saved
- 🐳 **Docker Ready**: Easy installation and execution with Docker

## Docker Installation

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

## Downloads

Executable files are available in the [Releases](https://github.com/mosqueiro/live-ai/releases) section for direct download.

## Configuration

1. Access the web interface at `http://localhost:8080`
2. Configure your YouTube credentials
3. Set streaming parameters
4. Start your AI-powered live stream!

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

In the [Releases](https://github.com/mosqueiro/live-ai/releases) section you'll find 4 different versions:

- **Docker** (Recommended): Use the `docker-compose.yml` for easier and isolated installation
- **macOS**: Executable binary for macOS
- **Linux**: Executable binary for Linux
- **Windows**: `.exe` executable for Windows

The Docker version is most recommended as it offers complete isolation and automatic configuration of persistent volumes.

## Support

For support and questions, open an issue in the GitHub repository.

## License

This project is licensed under the MIT License.
