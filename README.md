# `arch-ansible`: Automated setup of my ArchLinux workstation

## What it does

These playbooks install and configure:

- Base packages and AUR support (via yay and ansible-aur)
- My dotfiles and shell environment
- Dev environments: JVM, Go, JS/TS
- Virtualization environments: docker, kubernetes, VMs (virtualbox, vagrant, packer)
- Editors: VSCode

## Prerequisites

Installed ArchLinux, with current user in sudoers

## Install

```bash
# Install prerequisites
./bootstrap.sh

# Install whole environment
ansible-playbook -i inventory playbooks/site.yml --ask-become-pass
```
