# Linux-HA-Cluster

Linux High Availability Cluster implementation and administration using PCS, Pacemaker, Corosync, GFS2, fencing, quorum, and shared storage on RHEL/CentOS environments with practical hands-on tutorials, failover configuration, troubleshooting, and enterprise clustering concepts.

---

# Repository Objective

This repository provides complete hands-on documentation and practical implementation guides for configuring and managing Linux High Availability (HA) clusters in enterprise environments.

The repository focuses on:

- High Availability Cluster setup
- PCS and Pacemaker administration
- Corosync cluster communication
- Shared storage configuration
- GFS2 clustered filesystem
- Resource failover configuration
- Fencing (STONITH)
- Cluster troubleshooting
- Production-ready HA concepts

---

# Technologies Covered

| Component | Description |
|---|---|
| PCS | Cluster management utility |
| Pacemaker | Resource management engine |
| Corosync | Cluster communication layer |
| GFS2 | Clustered shared filesystem |
| Fence Agents | Node fencing and isolation |
| PCSD | Web-based cluster management |

---

# Supported Platforms

- RHEL 7 / RHEL 8
- CentOS
- Rocky Linux
- AlmaLinux
- Oracle Linux (OEL)

---

# Repository Structure

```text
Linux-HA-Cluster/
│
├── 01-Cluster-Architecture
├── 02-Initial-Node-Configuration
├── 03-YUM-Repository-Setup
├── 04-PCS-Installation
├── 05-Cluster-Authentication
├── 06-Cluster-Creation
├── 07-Corosync-Configuration
├── 08-Pacemaker-Management
├── 09-Cluster-Resources
├── 10-Fencing-Configuration
├── 11-GFS2-Setup
├── 12-Shared-Storage
├── 13-Quorum-and-Voting
├── 14-Failover-Testing

Topics Covered
-Cluster Fundamentals
-HA Architecture
-Active-Passive Cluster
-Active-Active Cluster
-Quorum Concepts
-Split Brain Prevention
-Cluster Communication

PCS Cluster Management
-PCS Installation
-Cluster Authentication
-Cluster Creation
-Node Management
-Cluster Startup & Shutdown
-Cluster Properties

Commands covered:
pcs cluster auth
pcs cluster setup
pcs cluster start
pcs cluster stop
pcs status
pcs config

Pacemaker Administration
-Resource Creation
-Resource Groups
-Constraints
-Failover Policies
-Resource Monitoring

Corosync Configuration
-Corosync Services
-Cluster Communication
-Multicast / Unicast Configuration
-Cluster Membership

Shared Storage & GFS2
-Shared Disk Configuration
-Multipath Concepts
-CLVM
-GFS2 Filesystem
-Clustered Mounting

Fencing (STONITH)
-Fence Device Configuration
-Node Isolation
-Cluster Protection
-Power Management

Cluster Resources
-Virtual IP Resources
-Filesystem Resources
-Apache/NFS Service Resources
-Resource Groups
-Resource Failover

Monitoring & Troubleshooting
-PCS Logs
-Corosync Logs
-Pacemaker Logs
-Cluster Recovery
-Node Failure Testing
-Service Failover Validation

Useful commands:
pcs status
journalctl -xe
crm_mon
corosync-cfgtool -s

PCS Web Interface
Manage cluster using web UI:
https://<node-ip>:2224


Features of This Repository
Step-by-step installation guides
Enterprise clustering concepts
Practical lab implementation
Production troubleshooting scenarios

Command references
Real-time examples

Shared storage configuration
GFS2 setup documentation
Use Cases

This repository is useful for:
Linux Administrators
RHCSA / RHCE / RHCA learners
DevOps Engineers
Infrastructure Engineers
Cluster Administrators
System Engineers


Prerequisites
Basic Linux administration knowledge
VirtualBox / VMware environment

Minimum two Linux nodes
Shared storage (optional for GFS2)
RHEL/CentOS ISO



Future Enhancements
Planned additions:
iSCSI shared storage setup
DRBD configuration
NFS HA cluster
apache HA cluster
MariaDB/MySQL HA
HAProxy cluster
Cluster automation using Ansible
Multi-node cluster configuration

Security Recommendations

Configure STONITH in production
Use dedicated heartbeat network
Enable SELinux policies
Restrict PCS web access
Configure firewall properly
Secure shared storage



Learning Goals
After completing this repository, users will be able to:

Build Linux HA clusters
Configure cluster resources
Implement failover mechanisms
Configure fencing
Manage clustered storage
Troubleshoot cluster failures
Monitor enterprise HA environments



Author
Abdul Rehan
GitHub Repository:
https://github.com/rehanadm/Linux-HA-Cluster

├── 15-Troubleshooting
└── README.md
