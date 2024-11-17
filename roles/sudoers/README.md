# Sudoers

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini sudoers.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-ol.ini sudoers.yaml -b
```

# K8s1 Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini sudoers.yaml -b
```

# OpenStack
```bash
ansible-playbook -i inventory/openstack.ini sudoers.yaml -b
```