# Install Prometheus Node Exporter

# NTP
```bash
ansible-playbook -i inventory/ntp.ini prometheus-node-exporter.yaml -b
```

# Proxmox
```bash
ansible-playbook -i inventory/proxmox.ini Ping.yaml -b
ansible-playbook -i inventory/proxmox.ini prometheus-node-exporter.yaml -b
```