# Fedora-Lab

> Documentation on my Fedora homeserver.

## Fundamentals

### Basics

This system runs on Fedora 41 Server, which means it automatically comes with Cockpit installed. Cockpit is a web interface for system administration.
I've added some extensions to Cockpit, namely [cockpit-file-sharing](https://github.com/45Drives/cockpit-file-sharing) and [cockpit-identities](https://github.com/45Drives/cockpit-identities).
These extensions help me with the management of users, groups and the setup of the SMB shares. More on that later.

### Docker

I try to run everything in Docker containers for convenience and I've installed Portainer as a frontend for easy management. I try to deploy every service or group of services in a stack with Docker-Compose, to keep everything nice and linked together. All the YAML configuration files for the stacks can be found in this repo.

## Applications

WIP
