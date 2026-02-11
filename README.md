# laravel-ubuntu-deployment

Deployment workspace for Laravel + Next.js projects on Ubuntu with Nginx, Supervisor, and Laravel Reverb (WebSocket).

## Supported platform
- Ubuntu 22.04 LTS
- Ubuntu 24.04 LTS
- PHP 8.4

## Workspace layout
- `deployment/common`
- Shared install/setup/security/supervisor/websocket notes and copy-paste command blocks.
- `deployment/projects/<domain>`
- Project-specific notes: database, repos, overview, commands, and Nginx site configs.

## Quick usage
1. Start with `deployment/common/command.text` for baseline server setup.
2. Use project-specific file `deployment/projects/<domain>/command.text`.
3. Enable Nginx configs from `deployment/projects/<domain>/nginx/` (`web.conf`, `api.conf`, `ws.conf`).
4. Run validation commands at the end of the command file.

## Security note
- Do not store real credentials in this repository.
- Use placeholders in `database.text` and keep real values in secure secret storage.
