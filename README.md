# Caddy Custom Builds

Custom [Caddy](https://caddyserver.com) Docker images with additional modules, built on hardened base images.

## Available Builds

### caddy-geoblock-crowdsec

Caddy with security and DNS modules:

- [caddy-dns/cloudflare](https://github.com/caddy-dns/cloudflare) - Cloudflare DNS provider
- [caddy-crowdsec-bouncer](https://github.com/hslatman/caddy-crowdsec-bouncer) - CrowdSec integration
- [caddy-ratelimit](https://github.com/mholt/caddy-ratelimit) - HTTP rate limiting
- [caddy-geoblock](https://github.com/anujc4/caddy-geoblock) - Geographic IP blocking

**Platforms:** `linux/amd64`, `linux/arm64`

**Pull:**

```bash
docker pull anujchandra/caddy-geoblock-crowdsec:latest
```

## Versioning

Every CI run bumps the patch version, pushes a `vX.Y.Z` git tag, and publishes both images tagged `X.Y.Z`, `latest`, and the commit SHA.

## License

MIT
