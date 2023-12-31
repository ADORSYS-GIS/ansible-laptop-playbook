# GIS Ansible Playbook

[![Ansible CI](https://github.com/ADORSYS-GIS/ansible-laptop-playbook/actions/workflows/ansible-ci.yml/badge.svg)](https://github.com/ADORSYS-GIS/ansible-laptop-playbook/actions/workflows/ansible-ci.yml)

This playbook is used to install and configure a GIS laptops.

## Requirements
- python3
- ansible

## Usage
```bash
ansible-galaxy collection install gis/laptop --upgrade
```

```bash
ansible-playbook -i hosts.ini gis.laptop.playbook --connection=local -e "nvm=true" -e "sdkman=true" --flush-cache
```