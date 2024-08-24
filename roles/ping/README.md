# Ping

# Proxmox
```bash
ansible-playbook -i inventory/proxmox.ini Ping.yaml -b
```

# Nexus
```bash
ansible-playbook -i inventory/nexus-ubuntu.ini Ping.yaml -b
```

# Graylog
```bash
ansible-playbook -i inventory/graylog-ubuntu.ini Ping.yaml -b
```

# Jenkins
```bash
ansible-playbook -i inventory/jenkins.ini Ping.yaml -kK -b
```

# Terraform
```bash
ansible-playbook -i inventory/terraform.ini Ping.yaml -b
```

# K8s1-OL
```bash
ansible-playbook -i inventory/k8s1-ol.ini Ping.yaml -b
```

# OCFS Ubuntu 22.04
```bash
ansible-playbook -i inventory/ocfs-ubuntu.ini Ping.yaml -b
```

# K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1-rhel.ini Ping.yaml -b
```

# Repository Ubuntu
```bash
ansible-playbook -i inventory/repository-ubuntu.ini Ping.yaml -b
```

# K8s1-Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini Ping.yaml -b
```

