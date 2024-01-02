# Delete Node

## K8s1-RHEL
#### Delete node Worker2
```bash
ansible-playbook -i inventory/k8s1_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_node=k8s-rhel-worker2.fillswim.local"
```

## K8s2-RHEL
#### Delete node Master2
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_node=k8s2-rhel-master2.fillswim.local"
```

#### Delete node Master3
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_node=k8s2-rhel-master3.fillswim.local"
```

#### Delete node Worker1
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_node=k8s2-rhel-worker1.fillswim.local"
```

#### Delete node Worker2
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_06-Delete-Node.yaml -b --extra-vars "deleted_node=k8s2-rhel-worker2.fillswim.local"
```
