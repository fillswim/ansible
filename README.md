![Ansible](images/Ansible_new.png)

# Ansible playbooks

### Deploy Nginx on K8s using Ansible playbook
```bash
ansible-playbook Helm_Template_Install.yml 
    --extra-var "helm_name=my-nginx 
                 helm_namespace=default 
                 file=/home/fill/K8SManifests/HelmChart_values_nginx.yaml"
```

### Deploy GifService on K8s using Ansible playbook
```bash
ansible-playbook Helm_Template_Install.yml 
    --extra-var "helm_name=my-gifservice 
                 helm_namespace=default 
                 file=/home/fill/K8SManifests/HelmChart_values_gifservice.yaml"
```

### General playbook

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini general.yaml -b
```

# Test Oracle
```bash
ansible-playbook -i inventory/test-oracle.ini general.yaml -b
```

# Repository Oracle
```bash
ansible-playbook -i inventory/repository-oracle.ini general.yaml -b
```
# K8s1 Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini general.yaml -b
```