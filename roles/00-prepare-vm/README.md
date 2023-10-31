
Первичная подготовка всех виртуальным машин:
```bash
ansible-playbook -i hosts_all.txt Roles_00-Prepare-VM.yaml -kK
```
```bash
ansible-playbook -i hosts_graylog_cluster_ubuntu.txt Roles_00-Prepare-VM.yaml -kK
```

Первичная подготовка виртуальным машин кластера K8s:
```bash
ansible-playbook -i hosts_k8s_alma.txt Roles_00-Prepare-VM.yaml -kK
```