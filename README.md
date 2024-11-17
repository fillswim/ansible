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

# MAAS
```bash
ansible-playbook -i inventory/maas.ini general.yaml -b
```

# OpenStack
```bash
ansible-playbook -i inventory/openstack.ini general.yaml -b
```

# K8s1-Ubuntu-Lab
```bash
ansible-playbook -i inventory/k8s1-ubuntu-lab.ini general.yaml -b
```

# NTP
```bash
ansible-playbook -i inventory/ntp.ini general.yaml -b
```

# Graylog
```bash
ansible-playbook -i inventory/graylog.ini general.yaml -b
```

# Minio
```bash
ansible-playbook -i inventory/minio-ubuntu.ini general.yaml -b
```

# K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1-rhel.ini general.yaml -b -kK
```

