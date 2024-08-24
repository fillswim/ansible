# Install packages

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini install.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-oracle.ini install.yaml -b
```

# K8s1 Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini install.yaml -b
```