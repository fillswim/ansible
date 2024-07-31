# Preparation General

# Nexus
```bash
ansible-playbook -i inventory/nexus-ubuntu.ini Preparation-General.yaml -b
```

# Graylog
```bash
ansible-playbook -i inventory/graylog-ubuntu.ini Preparation-General.yaml -b
```

# Jenkins:
```bash
ansible-playbook -i inventory/jenkins.ini Preparation-General.yaml -kK -b
```

# K8s1-RHEL:
```bash
ansible-playbook -i inventory/k8s1-rhel.ini Preparation-General.yaml -b
```

# K8s1-OL:
```bash
ansible-playbook -i inventory/k8s1-ol.ini Preparation-General.yaml -b
```

# OCFS Ubuntu:
```bash
ansible-playbook -i inventory/ocfs-ubuntu.ini Preparation-General.yaml -kK
```

# Nexus:
```bash
ansible-playbook -i inventory/nexus.ini Preparation-General.yaml -b
```

# Repository Ubuntu:
```bash
ansible-playbook -i inventory/repository-ubuntu.ini Preparation-General.yaml -b
```

# Repository Oracle Linux:
```bash
ansible-playbook -i inventory/repository-ol.ini Preparation-General.yaml -b
```

# Test Oracle Linux:
```bash
ansible-playbook -i inventory/test-ol.ini Preparation-General.yaml -b
```

