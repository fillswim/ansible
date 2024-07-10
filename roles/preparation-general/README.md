# Preparation General

# Graylog-Ubuntu
```bash
ansible-playbook -i inventory/graylog-ubuntu.ini Preparation-General.yaml -kK
```

# K8s1-RHEL:
```bash
ansible-playbook -i inventory/k8s1-rhel.ini Preparation-General.yaml -kK
```

# K8s1-OL:
```bash
ansible-playbook -i inventory/k8s1-ol.ini Preparation-General.yaml -kK
```

# OCFS Ubuntu:
```bash
ansible-playbook -i inventory/ocgs-ubuntu.ini Preparation-General.yaml -kK
```

# Nexus:
```bash
ansible-playbook -i inventory/nexus.ini Preparation-General.yaml -b
```