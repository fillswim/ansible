# Proxy repository

# Jenkins
```bash
ansible-playbook -i inventory/jenkins.ini Proxy-repository.yaml -kK -b
```

# Graylog
```bash
ansible-playbook -i inventory/graylog-ubuntu.ini Proxy-repository.yaml -b
```