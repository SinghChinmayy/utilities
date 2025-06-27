# utilities

This repo contains my bash scripts and other utilities.

## Caddy + Tailscale Quickstart

You can use [Caddy](./apps/caddy/notes) to easily serve static sites or files over your Tailscale network.

**Example Caddyfile for Tailscale:**
```caddyfile
[your-host-name].ts.net {
    root * /workspace/codes/sample_site/
    file_server
}
```

- Replace `[your-host-name].ts.net` with your actual Tailscale hostname (find it with `tailscale status`).
- This setup lets you securely share static sites or files across your Tailscale network with minimal configuration.

> **Note:**  
> The first time you access your `.ts.net` address, it may take a little longer as Caddy acquires a certificate for your Tailscale domain.

See [apps/caddy/notes](./apps/caddy/notes) for more Caddy usage and tips.
