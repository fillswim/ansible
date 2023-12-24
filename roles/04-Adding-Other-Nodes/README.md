# Add all other nodes to Cluster (by default - all nodes)
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b
```

# Add only one Master node
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b --extra-vars "added_node=k8s2-rhel-master3.fillswim.local"
```

# Add only one Worker node
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Nodes.yaml -b --extra-vars "added_node=k8s2-rhel-worker2.fillswim.local"
```