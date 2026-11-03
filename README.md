
# Self-Hosted Home Lab

**Architecture:** Two Physical Nodes | Dedicated VLAN | ZimaOS Compute Host | ZFS NAS

**Technologies:** ZimaOS, Docker, Portainer, ZFS, Linux, Windows 11, Virtualization, Networking

## Overview

I built and maintain a self-hosted home lab to develop hands-on experience with computer hardware, networking, virtualization, and infrastructure management.

The environment consists of two physical nodes: a ZimaOS compute server and a separate Network Attached Storage (NAS) system utilizing the ZFS filesystem. Both operate within a dedicated, segmented home-lab VLAN.

This project allows me to deploy applications, manage hardware resources, troubleshoot networking issues, and explore how different components of a computing infrastructure interact.

## System Architecture

The home lab consists of three primary components:

- **Compute Node (ZimaOS):** Hosts Docker containers and two virtual machines running Windows 11 and Ubuntu.
- **Storage Node (ZFS NAS):** Provides dedicated disk management and network-attached storage.
- **Network Infrastructure:** Uses a dedicated VLAN, static IP configuration, and router-level port forwarding for selected services.

[View Network and System Architecture Diagram](diagrams/homelab_overview.pdf)

## Services and Technologies

| Component | Purpose |
| --- | --- |
| Docker | Containerized application deployment |
| Portainer | Container management and monitoring |
| Plex | Self-hosted media streaming |
| Immich | Self-hosted photo and video management |
| Ollama | Local large language model experimentation |
| Cloudflared | Cloudflare Tunnel connectivity |
| Windows 11 VM | Windows application testing |
| Ubuntu VM | Linux experimentation and administration |
| ZFS NAS | Dedicated storage and filesystem management |

## Infrastructure Management

Managing this environment involves maintaining containerized services, configuring network access, monitoring resource utilization, and diagnosing problems across operating systems and applications.

Portainer provides centralized container management and access to application logs. The separate storage system allows compute and storage responsibilities to be managed independently.

## Networking and Security

- Implemented a dedicated VLAN to segment home-lab infrastructure from other network devices.
- Configured static IP assignments to maintain predictable network addressing.
- Implemented router-level port forwarding for services requiring external accessibility.
- Utilized Cloudflared for tunneling and remote-access configurations.
- Excluded private addresses, credentials, and sensitive configuration information from public documentation.

## Documentation

- [Operations Overview](docs/operations_overview.md)
- [Future Expansion Roadmap](docs/future_expansion.md)
- [System Architecture Diagram](diagrams/homelab_overview.pdf)

## Key Engineering Takeaways

- Gained hands-on experience operating a two-node computing and storage environment.
- Applied VLAN segmentation, static IP addressing, and port forwarding in a real network.
- Strengthened troubleshooting skills through container management, system monitoring, and log analysis.
- Developed familiarity with ZFS-based storage, virtualization, Linux administration, and infrastructure documentation.

**Project Scope:** Personal infrastructure and engineering experimentation environment.
