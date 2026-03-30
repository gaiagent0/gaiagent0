<div align="center">

# Istvan — gaiagent0

**Homelab architect · Self-hosted AI · Proxmox 3-node + Snapdragon X Elite ARM64 + OCI**

[![Repos](https://img.shields.io/badge/public_repos-17-blue?style=flat-square)](https://github.com/gaiagent0?tab=repositories)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](https://opensource.org/licenses/MIT)

</div>

---

## About

Self-hosted homelab on a **3-node Proxmox VE cluster** (Intel N100/N305 mini-PCs) and a **Snapdragon X Elite ARM64 laptop**.
OCI Always Free VMs for public-facing apps. Focus: reliable infrastructure, local AI inference, privacy-first self-hosting.

- 20+ LXC containers across 3 Proxmox nodes
- Local LLM: Ollama (CPU/GGUF) + Qualcomm NPU (QNN/ONNX, ~60 tok/s)
- 3-2-1 backup: PBS → pCloud via rclone
- LiteLLM gateway: 16 000+ free cloud req/day + local fallback
- OCI Always Free: FastAPI + Caddy + Qwen AI apps

---

## Repositories

### AI & Local Inference

| Repo | Description |
|---|---|
| [homelab-ai-stack](https://github.com/gaiagent0/homelab-ai-stack) | Ollama + Open WebUI + ChromaDB + n8n on Snapdragon ARM64 WSL2 |
| [snapdragon-ai-stack](https://github.com/gaiagent0/snapdragon-ai-stack) | NPU setup, RAG pipeline, model tiers, WSL2 Docker |
| [litellm-local-config](https://github.com/gaiagent0/litellm-local-config) | LiteLLM proxy: 16K free req/day + local fallback |
| [windows-ai-autostart](https://github.com/gaiagent0/windows-ai-autostart) | WSL2 + Docker autostart via Task Scheduler XML |

### Proxmox Homelab

| Repo | Description |
|---|---|
| [homelab-core-services](https://github.com/gaiagent0/homelab-core-services) | AdGuard, Nginx PM, VaultWarden, Tailscale on LXC |
| [homelab-monitoring-stack](https://github.com/gaiagent0/homelab-monitoring-stack) | LibreNMS + Grafana + Prometheus + Node Exporter |
| [homelab-backup-stack](https://github.com/gaiagent0/homelab-backup-stack) | PBS + rclone → pCloud, host bind-mount design |
| [homelab-media-stack](https://github.com/gaiagent0/homelab-media-stack) | Jellyfin + *arr + qBittorrent/Gluetun VPN |
| [proxmox-cluster-hardening](https://github.com/gaiagent0/proxmox-cluster-hardening) | e1000e EEE fix, r8169 fix, quorum auto-recovery |

### OCI Cloud Apps

| Repo | Description |
|---|---|
| [infra-insight](https://github.com/gaiagent0/infra-insight) | AI DevOps dashboard: server metrics + Qwen AI analysis |
| [hu-ai-chat](https://github.com/gaiagent0/hu-ai-chat) | Hungarian AI chat app: FastAPI + Qwen, OCI hosted |
| [yumma-chat](https://github.com/gaiagent0/yumma-chat) | WordPress AI chat plugin for yummatea.hu WooCommerce |

### Other

| Repo | Description |
|---|---|
| [fastmcp](https://github.com/gaiagent0/fastmcp) | fastmcp project |
| [my-page](https://github.com/gaiagent0/my-page) | my-page project |
| [portfolio](https://github.com/gaiagent0/portfolio) | portfolio project |
| [snapdragon_AI](https://github.com/gaiagent0/snapdragon_AI) | snapdragon_AI project |

---

## Tech Stack

`Proxmox VE` `LXC` `Docker` `WSL2` `Ollama` `LiteLLM` `Grafana` `Prometheus` `LibreNMS`
`AdGuard` `Nginx PM` `VaultWarden` `Tailscale` `Jellyfin` `PBS` `rclone`
`FastAPI` `Python` `Caddy` `OCI` `Qwen AI` `WordPress`
`PowerShell` `Bash` `systemd` `MikroTik RouterOS`