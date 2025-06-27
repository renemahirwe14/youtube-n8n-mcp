# 🚀 n8n + MCP Server Deployment Stack

This repository contains a fully containerized deployment stack for:

- 🧠 [**n8n**](https://n8n.io/) — a powerful workflow automation tool
- 🎬 **MCP Server** — a short-video generation microservice based on the `gyoridavid/short-video-maker` Docker image

Both services are configured for **zero-maintenance**, **always-on deployment** using [Coolify](https://coolify.io) on a VPS like AWS Lightsail.

---

## 📦 Stack Overview

| Service | Description | Port |
|--------|-------------|------|
| `n8n` | Workflow automation platform with basic auth | `5678` |
| `mcp` | AI-powered short video maker (with Pexels API) | `3123` |

---

## 🌐 Access After Deployment

After deploying via Coolify:

- 👉 **n8n:** `http://<-server-ip>:5678`
- 👉 **MCP:** `http://<-server-ip>:3123`

---

## 🛠 Prerequisites

To use this repo:

- A VPS with Docker & Coolify installed (e.g. Ubuntu on AWS Lightsail)
- A working [Coolify instance](https://docs.coollabs.io/coolify/) (port 3000 open)
- A [GitHub account](https://github.com/) to host this repository
- A free [Pexels API key](https://www.pexels.com/api/)

---

## 🚀 Deployment Instructions

### 1. Clone or Fork This Repo

```bash
git clone https://github.com/renemahirwe14/youtube-n8n-mcp.git
cd youtube-n8n-mcp
