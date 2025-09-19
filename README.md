# Ship Proxy System

This project implements a two-tier proxy system for enabling ships (with limited network access) to tunnel traffic securely through an offshore server.

## Features
- HTTP and HTTPS proxy support (via CONNECT tunneling)
- Works with `curl` or browsers configured to use proxy
- Supports forwarding normal HTTP requests
- Handles HTTPS encrypted traffic using framed tunneling
- Easy to run via Docker or Python

---

## Setup & Run

### 1. Offshore Proxy (runs on a server or WSL/Linux terminal)
```bash
python3 server.py --host 0.0.0.0 --port 9999
