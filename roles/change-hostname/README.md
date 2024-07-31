# Change hostname

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini change-hostname.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-ol.ini change-hostname.yaml -b
```