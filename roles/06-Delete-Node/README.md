# Delete node Master3
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_nodes=k8s2-rhel-master3.fillswim.local"
```

# Delete node Worker1
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_nodes=k8s2-rhel-worker1.fillswim.local"
```

# Delete node Worker2
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_nodes=k8s2-rhel-worker2.fillswim.local"
```
