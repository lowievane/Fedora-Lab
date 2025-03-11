# Fedora-Lab

> Documentation on my Fedora homeserver.

## Fundamentals

### Basics

This system runs on Fedora 41 Server, which means it automatically comes with Cockpit installed. Cockpit is a web interface for system administration.
I've added some extensions to Cockpit, namely [cockpit-file-sharing](https://github.com/45Drives/cockpit-file-sharing) and [cockpit-identities](https://github.com/45Drives/cockpit-identities).
These extensions help me with the management of users, groups and the setup of the SMB shares. More on that later.

### Docker

I try to run everything in Docker containers for convenience and I've installed Portainer as a frontend for easy management. I try to deploy every service or group of services in a stack with Docker-Compose, to keep everything nice and linked together. All the YAML configuration files for the stacks can be found in this repo.

### SMB shares
I've configured 3 SMB shares using Cockpit with the extensions mentioned earlier.
- Data share: for all kinds of random data and media files.
- Docker share: for all Docker container configurations. I put all Docker files in /opt/docker/\<container\>, this complete directory is also a share.
- LocalData share: another data share but on a different drive.

## Applications

Below you can find all applications I run, all with their seperate documentation.

### System

- Cockpit (see Fundamentals>Basics) 
- Portainer (see Fundamentals>Docker)
- [Nginx Proxy Manager](docs/nginxproxymanager.md)

### Media

- [Deluge](docs/deluge.md)
- [Jellyfin](docs/jellyfin.md)

### Monitoring

- [Prometheus](docs/prometheus.md)
- [Grafana](docs/grafana.md)
