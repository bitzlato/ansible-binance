# Ansible Role: Binance Smart Chain Fullnode 
Installs Binance Smart Chain Fullnode on Debian/Ubuntu servers.

This role installs and configures Binance Smart Chain Fullnode. You will likely need to do extra setup work before this role has installed Binance Smart Chain Fullnode, like changing  binance_httphost variabel, describing the location and options to use for your particular node.

# Requirements
1TB of free disk space

# Role Variables
Available variables are listed below, along with default values (see defaults/main.yml):

```
binance_httphost: '127.0.0.1'
```
Which IP address will be listening, default 127.0.0.1

```
binance_httpport: 8545
binance_wsport: 8546
```
Port connection options

# Example Playbook
```
- hosts: server
  become: yes
  roles:
    - ansible-binance
```
