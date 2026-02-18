# Operations Overview

## Environment Summary

The home lab operates on a single bare-metal system running ZimaOS. 
Containerized services are deployed as individual Docker containers and managed through Portainer. 
Two virtual machines (Windows 11 and Ubuntu) are hosted alongside container workloads for isolation and testing purposes.

---

## Network Configuration

To ensure stable service accessibility:

- Static IP assignments were configured for critical services (e.g., Plex).
- Router-level port forwarding was implemented where required for external access.
- NAT behavior was validated to ensure consistent routing and discovery.

This configuration improves service reliability by preventing IP reassignment and minimizing access interruptions.

---

## Container Management Strategy

Services are deployed as individual Docker containers rather than a single compose stack to:

- Maintain service isolation
- Allow independent restarts and updates
- Simplify troubleshooting workflows

Portainer is used to:

- Monitor container health
- Manage lifecycle operations (start/stop/redeploy)
- Inspect logs for debugging

Routine updates and version checks are performed to maintain system stability.

---

## Virtualization Strategy

Two virtual machines are maintained for controlled experimentation:

- Windows 11 VM — application testing and Windows-specific workflows
- Ubuntu VM — Linux experimentation, scripting, and service validation

Virtualization allows workload isolation without impacting containerized production-style services.

---

## Security Considerations

- Public IP addresses, credentials, and secrets are intentionally excluded from repository documentation.
- Port forwarding is limited to required services only.
- Cloudflared is used for controlled remote access scenarios (deployment details intentionally abstracted).

The system is designed with a local-network-first mindset, minimizing unnecessary service exposure.
