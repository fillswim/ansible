Proxmox VM Action

# Start
```bash
ansible-playbook -i inventory/proxmox.ini Proxmox-VM-Action.yaml --extra-vars "vm_action=started" --ask-vault-pass
```

# Reboot
```bash
ansible-playbook -i inventory/proxmox.ini Proxmox-VM-Action.yaml --extra-vars "vm_action=restarted" --ask-vault-pass
```

# Shutdown
```bash
ansible-playbook -i inventory/proxmox.ini Proxmox-VM-Action.yaml --extra-vars "vm_action=stopped" --ask-vault-pass
```