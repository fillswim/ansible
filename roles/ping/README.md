# Ping

#### all-vms
```bash
ansible-playbook -i inventory/all_vms.ini Role_Ping.yaml -b
```

#### K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1_rhel.ini Role_Ping.yaml -b
```

#### Nexus
```bash
ansible-playbook -i inventory/nexus.ini Role_Ping.yaml -b
```