#### K8s1-RHEL:
```bash
ansible-playbook -i inventory/k8s1_rhel.ini Role_NTP.yaml -b
```

#### All VMs:
```bash
ansible-playbook -i inventory/all_vms.ini Role_NTP.yaml -b
```