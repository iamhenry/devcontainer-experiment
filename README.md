# Devcontainer + OpenCode Template

A minimal devcontainer configuration for using [OpenCode CLI](https://opencode.ai) in a containerized development environment.

## What's Included

- TypeScript/Node.js base image
- OpenCode CLI (AI coding assistant)
- tmux for terminal multiplexing
- Common dev utilities

## Quick Start

1. Open this repository in VS Code
2. When prompted, click "Reopen in Container"
3. OpenCode will be available immediately via `opencode` command

## Configuration

The devcontainer mounts your local configs so your preferences carry over:

| Host Path | Container Path | Purpose |
|-----------|----------------|---------|
| `~/.opencode` | `/home/node/.opencode` | OpenCode settings |
| `~/.config/opencode` | `/home/node/.config/opencode` | OpenCode config |
| `~/.tmux.conf` | `/home/node/.tmux.conf` | tmux settings |
| `~/.local` | `/home/node/.local` | Local data |
| `~/bin` | `/home/node/bin` | Custom binaries |

## Requirements

- Docker
- VS Code with Dev Containers extension (or compatible IDE)

## Usage

Once inside the container:

```bash
# Start OpenCode
opencode
```

## License

MIT
