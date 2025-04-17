# n8n Backup

This repository contains backup files for n8n configuration and workflows. Sensitive information and credentials are excluded for security reasons.

## Directory Structure

- `/workflows` - n8n workflow configurations
- `/config` - Configuration files (excluding sensitive data)
- `/ssh` - SSH related configurations (excluding private keys)

## Security Notice

This repository excludes:
- Database files
- Log files
- Private keys and credentials
- Environment variables
- Sensitive configuration data

## Restore Process

1. Clone this repository
2. Copy the files to your n8n configuration directory (typically `~/.n8n/`)
3. Set up your credentials and sensitive configurations manually
4. Restart n8n

## Important

Always verify that no sensitive information is included before pushing changes to this repository. 