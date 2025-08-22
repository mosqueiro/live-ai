# Live AI - Intelligent YouTube Streaming

Live AI is an innovative YouTube streaming software that uses artificial intelligence to automate and optimize your live streams.

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

### ⚠️ **MUITO IMPORTANTE: Persistent Volumes**

**⚠️ ATENÇÃO: Se você não configurar os volumes persistentes, TODOS os seus dados serão perdidos quando o container for reiniciado!**

Application data is saved in the host's `./data` folder, mapped to `/app/data` in the container, ensuring your settings are maintained even after restarts.

**Por que é crucial:**

- Sem volumes persistentes, suas configurações do YouTube serão perdidas
- Seus dados de streaming e histórico serão apagados
- Você precisará reconfigurar tudo novamente a cada reinicialização

## Downloads

Executable files are available in the [Releases](https://github.com/mosqueiro/live-ai/releases) section for direct download.

## Configuration

1. Access the web interface at `http://localhost:8080`
2. Configure your YouTube credentials
3. Set streaming parameters
4. Start your AI-powered live stream!

## Instalação por Sistema Operacional

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

## Versões Disponíveis

No [Releases](https://github.com/mosqueiro/live-ai/releases) você encontrará 4 versões diferentes:

- **Docker** (Recomendado): Use o `docker-compose.yml` para instalação mais fácil e isolada
- **macOS**: Binário executável para macOS
- **Linux**: Binário executável para Linux
- **Windows**: Executável `.exe` para Windows

A versão Docker é a mais recomendada pois oferece isolamento completo e configuração automática dos volumes persistentes.

## Support

For support and questions, open an issue in the GitHub repository.

## License

This project is licensed under the MIT License.
