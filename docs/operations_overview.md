
# Home Lab Operations Overview

## Purpose

This document describes the architecture, configuration, and management practices used within my self-hosted home lab.

## Hardware and Platform Configuration

The environment consists of two physical machines:

1. **ZimaOS Compute Host:** Runs individual Docker containers alongside Windows 11 and Ubuntu virtual machines.
2. **ZFS NAS:** A separate network-attached storage system responsible for managing storage drives and the ZFS filesystem.

Separating compute and storage provides opportunities to experiment with resource management, infrastructure configuration, and troubleshooting across multiple machines.

## Network Configuration

The home lab operates within its own dedicated VLAN, separating its infrastructure from other devices on the home network.

Additional networking configurations include:

- Static IP assignments for predictable device addressing.
- Router-level port forwarding for selected externally accessible services.
- NAT and network routing configuration.
- Cloudflared connectivity for applicable remote-access services.

These configurations provide practical experience with network segmentation, addressing, service availability, and security.

## Container Management

Applications are deployed as individual Docker containers and managed primarily through Portainer.

Portainer is used to:

- Monitor container status and resource utilization.
- Start, stop, and restart services.
- Inspect application logs when diagnosing problems.
- Manage application configuration and lifecycle operations.

Deployed applications include Plex, Immich, Ollama, and Cloudflared.

## Virtualization

The ZimaOS compute host runs two virtual machines:

- **Windows 11:** Windows application testing and experimentation.
- **Ubuntu:** Linux administration, scripting, and software experimentation.

Virtualization provides isolated operating environments without requiring dedicated physical hardware for each system.

## Storage Architecture

A separate NAS manages the home lab's storage drives using ZFS.

This arrangement separates storage administration from application and compute workloads and provides experience with dedicated network storage infrastructure.

## Security Considerations

- Sensitive credentials and access tokens are excluded from public documentation.
- The home lab operates within a dedicated VLAN.
- External service exposure is limited to configured access methods.
- Private IP addresses, hostnames, and internal network details are not publicly documented.

## Troubleshooting Approach

When diagnosing infrastructure problems, I examine:

1. Container and application logs.
2. CPU, memory, and storage resource utilization.
3. Network configuration and service accessibility.
4. Host operating system behavior.
5. Storage availability and connectivity.

This systematic approach helps identify problems across multiple infrastructure layers.

## Project Scope

The current environment contains two physical nodes with separate compute and storage responsibilities. It is not designed or represented as a high-availability computing cluster.
