# Selfhosted
My approach to self-hosting. Single node (no k8s or Docker Swarm).

### Core ingredients
- Docker/Compose
- [Dockge](https://github.com/louislam/dockge): Docker compose stack-oriented manager. Alternative to portainer.
- [Caddy](https://github.com/caddyserver/caddy): Reverse proxy with automatic HTTPS.
- [caddy-docker-proxy](https://github.com/lucaslorentz/caddy-docker-proxy): Caddy as a reverse proxy for Docker, via labels. Light alternative to Traefik.
- [Tailscale](https://github.com/tailscale/tailscale): Private WireGuard network made easy. To access my server from anywhere, securely.
- [Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/): To expose some services to the world.
- [Reaction](https://framagit.org/ppom/reaction): Scan logs and take action. As an alternative to fail2ban.

## TODO
- [ ] Don't share same network beteewn Caddy and rest of containers
- [ ] Use Caddy auto-https
- [ ] Authelia
- [ ] `reaction` to vaultwarden repeated wrong passwords
- [ ] `reaction` to sub-domain enumeration
- [ ] Tailscale split DNS

