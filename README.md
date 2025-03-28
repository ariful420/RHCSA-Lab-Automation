# RHCSA Lab Automation

This project automates the setup of a RHCSA lab environment using Rocky Linux in a virtualized setup (KVM, VirtualBox, or Docker).

## Features

- Automated installation of Rocky Linux in a VM (with cloud-init)
- Pre-configured users & groups (/etc/passwd, /etc/group, /etc/shadow)
- Filesystem setup (LVM, partitions, ext4, XFS)
- Firewall & SELinux configurations
- Automated package installations (dnf/yum setup)
- Network setup (static IP, hostname, DNS, DHCP)
- Backup & Restore system state
- Automated user permissions & ACLs

## Tech Stack

- Bash scripting (for automation)
- Python (Fabric/Paramiko) (for remote execution)
- Ansible (for configuration management)

## Repository Structure

```plaintext
RHCSA-Lab-Automation/
│── scripts/
│   ├── install_rocky.sh
│   ├── setup_users.sh
│   ├── configure_firewall.sh
│── ansible/
│   ├── playbook.yml
│── docs/
│   ├── README.md
│   ├── setup_guide.md
```

## Why This Project?

- Helps RHCSA candidates easily practice on a real system
- Demonstrates automation & system admin skills
- Useful for home labs & IT training

## Getting Started

### Prerequisites

- A virtualization platform (KVM, VirtualBox, or Docker)
- Python 3.x
- Ansible
- Fabric/Paramiko

### Installation

1. Clone the repository
    ```bash
    git clone https://github.com/your-username/RHCSA-Lab-Automation.git
    cd RHCSA-Lab-Automation
    ```

2. Follow the setup guide in `docs/setup_guide.md` to prepare your environment.

### Usage

1. Run the installation script
    ```bash
    bash scripts/install_rocky.sh
    ```

2. Run the Ansible playbook
    ```bash
    ansible-playbook ansible/playbook.yml
    ```

For detailed instructions, refer to the `docs/setup_guide.md`.

## Contributing

Contributions are welcome! Please read the [contributing guidelines](docs/CONTRIBUTING.md) first.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
