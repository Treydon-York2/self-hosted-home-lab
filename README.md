Self-Hosted Home Lab Project

ENVIRONMENT:
Single-node bare-metal server running ZimaOS; Docker containers managed via Portainer

OVERVIEW:
Designed and maintained a self-hosted home lab to deploy and operate local network services while developing hands-on infrastructure skills in Linux, networking, virtualization, and container operations.

ARCHITECTURE:
A high-level topology diagram is available here - diagrams/homelab_overview.pdf

SERVICES DEPLOYED:
* Plex - media streaming; configured with static IP and router port forwarding for reliable access
* Immich - self-hosted photo management (local-first storage)
* Ollama - local LLM runtime for experimentation
* Cloudflared - secure access/tunneling component

PLATFORM & TOOLING:
* ZimaOS (bare metal host/hypervisor)
* Docker (individual containers)
* Portainer (container management)
* Virtual Machines (Windows 11 and Ubuntu VM's)

OPERATIONS & RELIABILITY:
* Configured static IP assignments for key services to ensure stable routing and discovery
* Implemented router port forwarding where needed for service accessibility
* Troubleshot using logs, resource monitoring, and network diagnostics (DNS, routing, port checks)

KEY TAKEAWAYS:
* Developed hands-on experience managing containerized services in a production-style Linux environment
* Strengthened understanding of network configuration, static IP assignment, and router-level port forwarding
* Built operational discipline around service uptime, troubleshooting, and log-based diagnostics
* Gained practical exposure to virtualization by maintaining isolated Windows and Linux environments
* Improved infrastructure reliability through structured service deployment and resource monitoring
