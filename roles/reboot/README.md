# Reboot

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini reboot.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-ol.ini reboot.yaml -b
```

# K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1-rhel.ini reboot.yaml -b
```