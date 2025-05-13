# home-data-server-setup
A documented setup of my personal Ubuntu-based analytics server. Runs JupyterLab, Python, and data science tools over SSH, powered by an AMD A8 with a 1050 Ti GPU.

## Hardware
- CPU: AMD A8-7600
- GPU: NVIDIA GTX 1050 Ti
- RAM: 8Gb
- OS: Ubuntu Server 22.04
- Network: Cudy AX210 Wi-Fi adapter

## Features
- JupyterLab with full Python data stack
- SSH access
- `tmux`-based long-running sessions
- Internet via Cudy AX210 (custom driver install)

## Step-by-Step Setup
  ### 1. Ubuntu Server Installation
    - Installed Ubuntu Server 22.04 LTS
    - No GUI, CLI-only
    - Installed with minimal packages
### 2. Network Setup
    - Configured `netplan` manually
    - Installed Cudy AX210 driver: [link to how you did this]
### 3. Package Installation
    ```bash
    sudo apt install python3-venv curl git fail2ban ufw

