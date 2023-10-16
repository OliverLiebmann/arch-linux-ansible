# Arch linux post-install with ansible
![Linting Status](https://github.com/OliverLiebmann/arch-linux-ansible/actions/workflows/ansible-lint.yml/badge.svg)

## Description
This Ansible playbook is designed for post-installation tasks on an Arch Linux system. It automates the configuration and installation of common packages and settings to streamline the setup process.

## Prerequisites
Before running this playbook, ensure you have the following prerequisites installed on your Arch Linux machine:

- Ansible
- Git
- Python

You can install these dependencies with the following command:

```bash
sudo pacman -S ansible git python
```

## Installation
To get started with this playbook, follow these steps:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/OliverLiebmann/arch-linux-ansible.git
   ```

2. Change into the project directory:

   ```bash
   cd arch-linux-ansible
   ```

3. Install required Ansible roles defined in `requirements.yml` using the following command:

   ```bash
   ansible-galaxy install -r requirements.yml
   ```

## Usage
To run the playbook, execute the following command from the project directory:

```bash
ansible-playbook main.yml --ask-become-pass
```

You will be prompted for the sudo password as the playbook requires elevated privileges to make system-level changes.