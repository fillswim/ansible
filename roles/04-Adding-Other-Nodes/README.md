# Add all other nodes to Cluster (by default - all nodes)
# Добавляются все ноды со всего кластера, если они уже не добавлены
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b
```

# Add only one Master node
# Добавление одной Master2 ноды
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b --extra-vars "added_node=k8s2-rhel-master2.fillswim.local"
```

# Добавление одной Master3 ноды
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b --extra-vars "added_node=k8s2-rhel-master3.fillswim.local"
```

# Add only one Worker1 node
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b --extra-vars "added_node=k8s2-rhel-worker1.fillswim.local"
```

# Add only one Worker2 node
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b --extra-vars "added_node=k8s2-rhel-worker2.fillswim.local"
```