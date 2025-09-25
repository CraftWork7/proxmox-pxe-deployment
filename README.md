# Proxmox 9 Deployment via PXE

Ansible playbook to configure a server that can be used to deploy Proxmox 9 via PXE boot. Tested on Rocky 9.


- Update inventory/inventory.yml
- Update inventory/groups_vars/all.yml

**Rocky 9 Instructions**

```bash
sudo dnf install epel-release -y
sudo dnf install ansible -y
ansible-galaxy collection install containers.podman
ansible-playbook playbooks/site.yml
```

