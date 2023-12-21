# Add all Worker nodes in [k8s_workers] to Cluster
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_05-Adding-Worker-Nodes.yaml -b
```

# Add node Worker1
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_05-Adding-Worker-Nodes.yaml -b --extra-vars "added_worker_nodes=k8s2-rhel-worker1.fillswim.local"
```

# Add node Worker2
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_05-Adding-Worker-Nodes.yaml -b --extra-vars "added_worker_nodes=k8s2-rhel-worker2.fillswim.local"
```