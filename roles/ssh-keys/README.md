# SSH-keys

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini ssh-keys.yaml -b
```

# Test Oracle Linux
```bash
ansible-playbook -i inventory/test-ol.ini ssh-keys.yaml -b
```

# K8s1 Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini ssh-keys.yaml -b
```