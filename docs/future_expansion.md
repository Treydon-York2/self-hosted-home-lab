
# Future Expansion Roadmap

This home lab is an ongoing personal engineering project. The following improvements are under consideration as opportunities to explore additional infrastructure and networking concepts.

## Advanced Network Segmentation

The current environment already uses a dedicated home-lab VLAN.

Future improvements may include:

- Creating additional VLANs for management, experimentation, and externally accessible services.
- Implementing more granular firewall and inter-VLAN routing policies.
- Documenting network access rules and segmentation behavior.

## Monitoring and Observability

Potential improvements include:

- Centralized CPU, memory, and storage monitoring.
- Container uptime and service availability dashboards.
- Automated alerts for abnormal resource utilization.
- Historical network and system performance logging.

## Backup and Recovery

Future work may involve:

- Developing automated backup schedules.
- Implementing additional off-site or external backup storage.
- Testing recovery procedures for important applications and configurations.
- Exploring ZFS snapshots and recovery workflows.

## Automated Container Deployment

Explore Docker Compose and version-controlled deployment configurations to improve:

- Deployment consistency.
- Service recovery and reconfiguration.
- Configuration documentation.
- Reproducibility across operating environments.

## Distributed Computing

Although the home lab currently contains two physical nodes, compute workloads are primarily handled by the ZimaOS server.

Future experimentation may involve:

- Adding an additional compute node.
- Distributing selected workloads across multiple hosts.
- Exploring load balancing and service availability.
- Testing container orchestration and recovery behaviors.

## Continuous Documentation

Maintain updated architecture diagrams, configuration notes, and sanitized screenshots as the infrastructure evolves.

Completed features and proposed improvements will continue to be documented separately.
