# Troubleshooting

Common issues and solutions for Live AI.

## Navigation

- [← Back to README](README.md)
- [🔑 Getting Your Free API Key](GETTING_API_KEY.md)
- [📖 Installation Guide](INSTALLATION.md)
- [🎥 YouTube Live Setup](YOUTUBE_LIVE.md)
- [⚙️ Configuration](CONFIGURATION.md)

## Common Issues

### Service Not Starting

**Problem**: The service doesn't start or is not accessible.

**Solutions**:

1. Check if Docker is running
2. Verify the port 8080 is not in use
3. Check Docker logs: `docker-compose logs live-ai`

### Data Loss

**Problem**: Settings and data are lost after restart.

**Solutions**:

1. Ensure persistent volumes are configured correctly
2. Check if the `./data` folder exists and has proper permissions
3. Verify the volume mapping in `docker-compose.yml`

### API Key Issues

**Problem**: API key not working or invalid.

**Solutions**:

1. Verify your API key at [https://live.1click.ai/](https://live.1click.ai/)
2. Check if the API key is correctly entered
3. Ensure the API key has proper permissions

### YouTube Stream Issues

**Problem**: Cannot connect to YouTube or stream fails.

**Solutions**:

1. Verify your YouTube stream key is correct
2. Check if the stream is scheduled and enabled
3. Ensure auto-start is enabled in YouTube Studio

## Getting Help

If you continue to experience issues:

1. Check the [Configuration](CONFIGURATION.md) guide
2. Review the [Installation](INSTALLATION.md) guide
3. Join our community: [https://www.skool.com/1clickai](https://www.skool.com/1clickai)

## Logs

To view system logs:

```bash
# Docker logs
docker-compose logs live-ai

# Follow logs in real-time
docker-compose logs -f live-ai
```
