# n8n Backup

This repository contains backup files for n8n configuration and workflows. Sensitive information and credentials are excluded for security reasons.

## Directory Structure

- `/workflows` - n8n workflow configurations
- `/custom` - Custom nodes and configurations
- `/config` - Configuration files (excluding sensitive data)
- `/ssh` - SSH related configurations (excluding private keys)

## Docker Deployment

This n8n instance is configured to run with Docker. To deploy:

1. Clone this repository
2. Copy the example environment file and configure your credentials:
   ```bash
   cp .env.example .env
   ```
3. Edit the `.env` file and add your API keys and credentials
4. Start the container:
   ```bash
   docker-compose up -d
   ```
5. Access n8n at http://localhost:5678

### Environment Variables

The following environment variables need to be configured:
- `MCP_OPENAI_API_KEY` - OpenAI API key
- `MCP_SERPER_API_KEY` - Serper API key
- `MCP_WEATHER_API_KEY` - Weather API key
- `MCP_BRAVE_API_KEY` - Brave API key

## Security Notice

This repository excludes:
- Database files
- Log files
- Private keys and credentials
- Environment variables
- Sensitive configuration data

## Restore Process

1. Clone this repository
2. Set up your environment variables in `.env`
3. Start the container with `docker-compose up -d`
4. Import your workflows through the n8n UI
5. Configure your credentials in the n8n UI

## Important

Always verify that no sensitive information is included before pushing changes to this repository. 