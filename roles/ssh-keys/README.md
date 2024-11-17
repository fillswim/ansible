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

# OpenStack
```bash
ansible-playbook -i inventory/openstack.ini ssh-keys.yaml -b -kK
```

# MAAS
```bash
ansible-playbook -i inventory/maas.ini ssh-keys.yaml -b -kK
```

# Lab
```bash
ansible-playbook -i inventory/k8s1-ubuntu-lab.ini ssh-keys.yaml -b
```