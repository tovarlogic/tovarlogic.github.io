---
title: Self hosting
lastmod: 2024-07-06T18:01:37.785Z
---

# Set-up the system
## update and upgrade
    sudo apt install
    sudo apt upgrade
## Fail2ban
1. installation
    apt install fail2ban
2. check service
    systemctl status fail2ban.service

# Clouddron.io
[Guide](https://docs.cloudron.io/)

## requirements 
1. OS: >= ubuntu 22.04
2. free for up to 2 apps

## update machine
    sudo apt update
## installation
    wget https://cloudron.io/cloudron-setup
    chmod +x ./cloudron-setup
    ./cloudron-setup 

## security hardening
### SSH
1. To disable password authentication, check for the following line in /etc/ssh/sshd_config:

    PasswordAuthentication no
    PermitRootLogin yes        # If set to 'yes', store the ssh keys in root user (/root/.ssh/authorized_keys)
                           # If set to 'no', store the ssh keys in sudo user (/home/ubuntu/.ssh/authorized_keys)

    By default, the SSH server runs on port 22. We recommend moving this to port 202 to prevent brute force attacks. Be careful to not lock yourself out when following the instructions below.

2. To change the SSH port, change the following line in /etc/ssh/sshd_config:

    Port 202   # Do not use any other port. Only this port is not blocked by the Cloudron firewall

# YUNOHOST
[Guide](https://yunohost.org/en/install/hardware:vps_debian)

## requirements
1. OS: Debian OS 11

## set-up
1. installation
    curl https://install.yunohost.org | bash
2. post-install
    - via web, or
    yunohost tools postinstall 
3. run diagnostics and fix issues
    - create dns records [guide](https://yunohost.org/en/dns_config)
    - create swap [guide](https://www.digitalocean.com/community/tutorials/how-to-add-swap-space-on-debian-11)


