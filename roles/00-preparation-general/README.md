
# Первичная подготовка всех виртуальным машин:
```bash
ansible-playbook -i inventory/all_vms.ini Role_00-Preparation-General.yaml -kK
```

# Graylog
```bash
ansible-playbook -i inventory/grl_ubuntu.ini Role_00-Preparation-General.yaml -kK
```

# K8s1-Alma:
```bash
ansible-playbook -i inventory/k8s1_alma.txt Role_00-Preparation-General.yaml -kK
```

# K8s1-RHEL:
```bash
ansible-playbook -i inventory/k8s1_rhel.ini Role_00-Preparation-General.yaml -kK
```

# K8s2-RHEL:
K8s2-RHEL:
```bash
ansible-playbook -i inventory/k8s2_rhel.ini Role_00-Preparation-General.yaml -kK
```