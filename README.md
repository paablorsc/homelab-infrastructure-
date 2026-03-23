# Homelab Infrastructure (Proxmox)

## Overview

This project documents a self-hosted homelab environment built on Proxmox.

The goal is to design and manage a small-scale infrastructure including virtualization, network services, secure remote access, and automation.

The environment simulates real-world system administration and infrastructure management using multiple virtual machines.

---

## Architecture

- Proxmox VE host running multiple virtual machines
- Services isolated across different VMs
- Internal network for service communication
- Secure remote access via Tailscale VPN

---

## Technologies

- Proxmox VE (virtualization platform)
- Pi-hole (DNS filtering and ad blocking)
- Tailscale (secure remote access VPN)
- Home Assistant (home automation platform)

---

## Infrastructure Design

### Virtualization Layer

- Proxmox used to manage virtual machines
- Each service runs in an isolated environment
- Resources allocated per service for stability

### Network Services

- Pi-hole configured as the main DNS resolver
- Blocks ads and tracking domains across the network
- Improves privacy and reduces unnecessary traffic

### Remote Access

- Tailscale provides secure remote access
- No port forwarding required
- Encrypted peer-to-peer communication

### Automation Layer

- Home Assistant used for smart device control
- Centralized automation and monitoring

---

## Key Features

- Self-hosted infrastructure
- Virtualized services on a single host
- Secure remote access without exposing ports
- Network-wide ad blocking
- Service isolation for stability and security

---

## Use Cases

- Secure remote access to home network
- Blocking ads and tracking domains on all devices
- Running multiple services efficiently on one machine
- Managing and automating smart home devices

---

## Screenshots

### Proxmox Dashboard
![Proxmox Dashboard](https://github.com/user-attachments/assets/9a88e85b-d42d-4ec6-9dc3-f82cdfa22ebe)

*Virtual machines managed through Proxmox interface*

---

### Pi-hole Dashboard
![Pi-hole Dashboard](https://github.com/user-attachments/assets/70c019d1-108f-41d1-8b1b-243dd78c0432)

*Network-wide DNS filtering and query statistics*

---

### Tailscale Devices
![Tailscale Devices](https://github.com/user-attachments/assets/4357e1df-d3d2-41a5-a53d-03879d1096d9)

*Devices connected through secure private VPN*

*Sensitive information has been removed for security reasons.*

---

### Home Assistant
![Home Assistant](https://github.com/user-attachments/assets/a5793d46-8510-40d7-bb1f-583c9ec366e9)

*Home Assistant running and ready for configuration*

---

## Future Improvements

- VLAN network segmentation
- Reverse proxy (NGINX / Traefik)
- Monitoring stack (Prometheus / Grafana)
- Centralized logging
- Automated backups

---

## Notes

All services are deployed in a controlled lab environment for learning, testing, and experimentation.
