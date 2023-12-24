# Add node Master3
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Control-Nodes.yaml -b --extra-vars "added_control_nodes=k8s2-rhel-master3.fillswim.local"
```

# Add all Worker nodes in [k8s_workers] to Cluster
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_04-Adding-Other-Control-Nodes.yaml -b
```