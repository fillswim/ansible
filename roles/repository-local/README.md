# Local repository

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini repository-local.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-oracle.ini repository-local.yaml -b
```

# K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1-rhel.ini repository-local.yaml -b -kK
```