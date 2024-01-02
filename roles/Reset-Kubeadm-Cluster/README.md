# Reset Cluster

## K8s1-RHEL:
```bash
ansible-playbook -i inventory/k8s1_rhel.yaml Role_Reset-Kubeadm-Cluster.yaml -b
```

## K8s2-RHEL:
```bash
ansible-playbook -i inventory/k8s2_rhel.yaml Role_Reset-Kubeadm-Cluster.yaml -b
```