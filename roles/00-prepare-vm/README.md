
Первичная подготовка всех виртуальным машин:
```bash
ansible-playbook -i hosts_all.txt Roles_00-Prepare-VM.yaml -kK
```
```bash
ansible-playbook -i hosts_graylog_cluster_ubuntu.txt Roles_00-Prepare-VM.yaml -kK
```
Ansible-clients:
```bash
ansible-playbook -i hosts_ansible_clients_ubuntu.txt Roles_00-Prepare-VM.yaml -kK
```
K8s-RHEL:
```bash
ansible-playbook -i hosts_k8s_rhel.ini Roles_00-Prepare-VM.yaml -kK
```

K8s2-RHEL:
```bash
ansible-playbook -i hosts_k8s2_rhel.ini Roles_00-Prepare-VM.yaml -kK
```

Первичная подготовка виртуальным машин кластера K8s:
```bash
ansible-playbook -i hosts_k8s_alma.txt Roles_00-Prepare-VM.yaml -kK
```