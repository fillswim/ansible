# Update

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini update.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-ol.ini update.yaml -b
```

# K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1-rhel.ini update.yaml -b
```