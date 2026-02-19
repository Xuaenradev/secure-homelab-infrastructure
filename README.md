# secure-homelab-infrastructure
My homelab infrastructure
This project documents the design and operation of a self-hosted Linux-based homelab environment used to simulate small-scale production infrastructure.

The environment is built using Docker containers and includes reverse proxy routing, monitoring, and service isolation.

Technologies Used

Linux (Arch-based)

Docker & Docker Compose

Nginx Proxy Manager

Prometheus

Grafana

AdGuard Home

Self-hosted services (Jellyfin, Immich, etc.)

Architecture

External Traffic
→ Reverse Proxy (Nginx Proxy Manager)
→ Internal Docker Network
→ Service Containers

Monitoring stack collects system metrics and container health.

Security Considerations

Reverse proxy used to centralize entry points

No unnecessary ports exposed

Docker network segmentation

DNS filtering via AdGuard Home

Regular container updates

Monitoring & Visibility

Prometheus collects metrics
Grafana dashboards visualize system health
Logs reviewed during troubleshooting events

Lessons Learned

Importance of proper port isolation

Reverse proxy reduces attack surface

Monitoring improves incident visibility

Permissions management in Linux is critical
