# Homelab

This repository documents my homelab environment, built on Proxmox and used to learn virtualisation, Linux, networking, automation, and cloud engineering concepts.

This homelab is where I build real hands on experience as I work toward becoming a cloud engineer.

Hardware ill be using:
-HP ProDesk 600 G5 Mini
-Intel i5-9500T
-16GB RAM
-512GB NVMe SSD
-External storage planned for media

Current Architecture

Proxmox host
This hypervisor will handle virtualisation, snapshots, networking, and storage. It is the core of the homelab and where I manage all other machines.

Lab VM (Ubuntu Server)
In this VM i will test things and try experiment with various tools without worrying about breaking anything important. Currently i have Docker, Portainer, Git, Terraform, and the AWS CLI installed.

I will also be separating the environment into logical parts. An infra/services VM for things like Tailscale, dashboards, monitoring, and general utility services, a media server VM that will run Jellyfin as well as a few lightweight LXC containers for specialised services like Pi-hole.

This separation is imperative and keeps the lab organised and makes it easier to troubleshoot or rebuild individual pieces.

My Progress So Far

Proxmox is fully installed and configured, including networking fixes and a stable SSH workflow from my Linux desktop.
I’ve created my main Lab VM and set up the core tools I’ll use moving forward.
Most of the initial legwork such as updates, users, SSH keys, Docker setup, Terraform installation is done, and now the environment is ready for building out proper services.

Future Plans

Once the homelab foundation is solid and I’m more confident with networking and AWS fundamentals, I’ll start building AWS projects. Each of those will live in its own separate repository

This repo will eventually include architecture diagrams, documentation for each service, notes, troubleshooting logs, and anything else related to the homelab. Subfolders will be added as the environment grows.

Last Thing

I strongly believe building and running my own virtualised environment forces me to learn Linux, networking, storage, containers, and infrastructure in a way that tutorials can’t teach. Every mistake becomes a lesson, and every service I deploy helps build the skills I need for real cloud work later. 

Self-hosting has already been challenging but extremely fulfilling, from SSH’ing into Proxmox from my desktop to watching services come alive as I configure them. And this is only the beginning of the journey.
