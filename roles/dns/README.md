# DNS

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini dns.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-oracle.ini dns.yaml -b
```

# K8s1 Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini dns.yaml -b
```