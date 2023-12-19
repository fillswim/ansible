
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_host=k8s2-rhel-worker2.fillswim.local"
```
