# General playbook

# ==================================================================================================
# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini general.yaml -b
```

# Test Oracle
```bash
ansible-playbook -i inventory/test-oracle.ini general.yaml -b
```

# ==================================================================================================

# NTP
```bash
ansible-playbook -i inventory/ntp.ini general.yaml -b
```

# DNS
```bash
ansible-playbook -i inventory/dns.ini ssh-keys.yaml -b -kK
ansible-playbook -i inventory/dns.ini ping.yaml -b
ansible-playbook -i inventory/dns.ini dns.yaml -b
ansible-playbook -i inventory/dns.ini repository-local.yaml -b
ansible-playbook -i inventory/dns.ini general.yaml -b
```

# Repository Ubuntu
```bash
ansible-playbook -i inventory/repository-ubuntu.ini general.yaml -b
```

# Repository Oracle
```bash
ansible-playbook -i inventory/repository-oracle.ini general.yaml -b
ansible-playbook -i inventory/repository-oracle.ini ping.yaml -b
ansible-playbook -i inventory/repository-oracle.ini prometheus-node-exporter.yaml -b
```

# Terraform Server
```bash
ansible-playbook -i inventory/terraform.ini general.yaml -b
```

# Minio
```bash
ansible-playbook -i inventory/minio.ini general.yaml -b
```

# Prometheus Server
```bash
ansible-playbook -i inventory/prometheus.ini general.yaml -b
ansible-playbook -i inventory/prometheus.ini prometheus-server.yaml -b
```

# Nexus
```bash
ansible-playbook -i inventory/nexus.ini general.yaml -b
```

# Graylog
```bash
ansible-playbook -i inventory/graylog.ini ping.yaml -b
ansible-playbook -i inventory/graylog.ini change-hostname.yaml -b
ansible-playbook -i inventory/graylog.ini repository-local.yaml -b
ansible-playbook -i inventory/graylog.ini general.yaml -b
```

# ==================================================================================================

# K8s1 Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini general.yaml -b
```

# MAAS
```bash
ansible-playbook -i inventory/maas.ini general.yaml -b
```

# OpenStack
```bash
ansible-playbook -i inventory/openstack.ini general.yaml -b
```

# K8s1-Ubuntu-Lab
```bash
ansible-playbook -i inventory/k8s1-ubuntu-lab.ini general.yaml -b
```

# K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1-rhel.ini general.yaml -b -kK
```



