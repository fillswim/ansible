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