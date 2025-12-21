# General playbook

```bash
source .venv/bin/activate
```

# ==================================================================================================
# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini general.yaml -b
```

# Test Oracle
```bash
ansible-playbook -i inventory/test-oracle.ini general.yaml -b
```

# ==================================================================================================

# NTP
```bash
ansible-playbook -i inventory/ntp.ini general.yaml -b
```

# DNS
```bash
ansible-playbook -i inventory/dns.ini ssh-keys.yaml -b -kK
ansible-playbook -i inventory/dns.ini ping.yaml -b
ansible-playbook -i inventory/dns.ini dns.yaml -b
ansible-playbook -i inventory/dns.ini repository-local.yaml -b
ansible-playbook -i inventory/dns.ini general.yaml -b
```

# Repository Ubuntu
```bash
ansible-playbook -i inventory/repository-ubuntu.ini general.yaml -b
```

# Repository Oracle
```bash
ansible-playbook -i inventory/repository-oracle.ini general.yaml -b
ansible-playbook -i inventory/repository-oracle.ini ping.yaml -b
ansible-playbook -i inventory/repository-oracle.ini prometheus-node-exporter.yaml -b
```

# Terraform Server
```bash
ansible-playbook -i inventory/terraform.ini general.yaml -b
```

# Jenkins
```bash
ansible-playbook -i inventory/jenkins.ini ssh-keys.yaml -b -kK
ansible-playbook -i inventory/jenkins.ini general.yaml -b
ansible-playbook -i inventory/jenkins.ini change-hostname.yaml -b
```

# Minio
```bash
ansible-playbook -i inventory/minio.ini general.yaml -b
```

# Prometheus Server
```bash
ansible-playbook -i inventory/prometheus.ini general.yaml -b
ansible-playbook -i inventory/prometheus.ini prometheus-server.yaml -b
```

# Nexus
```bash
ansible-playbook -i inventory/nexus.ini general.yaml -b
```

# Graylog
```bash
ansible-playbook -i inventory/graylog.ini ping.yaml -b
ansible-playbook -i inventory/graylog.ini change-hostname.yaml -b
ansible-playbook -i inventory/graylog.ini repository-local.yaml -b
ansible-playbook -i inventory/graylog.ini general.yaml -b
```

# Test Ubuntu
```bash
ansible-playbook -i inventory/test-ubuntu.ini ping.yaml -b
ansible-playbook -i inventory/test-ubuntu.ini general.yaml -b
ansible-playbook -i inventory/test-ubuntu.ini install-promtail-agent.yaml -b
```

# GitLab Runners
```bash
ansible-playbook -i inventory/gitlab-runners.ini general.yaml -b
ansible-playbook -i inventory/gitlab-runners.ini Install-Docker.yaml -b
```

# OpenStack
```bash
ansible-playbook -i inventory/openstack.ini ping.yaml -b
ansible-playbook -i inventory/openstack.ini chrony.yaml -b
ansible-playbook -i inventory/openstack.ini timezone.yaml -b
ansible-playbook -i inventory/openstack.ini sudoers.yaml -b
ansible-playbook -i inventory/openstack.ini ssh-keys.yaml -b
ansible-playbook -i inventory/openstack.ini ssh-keys.yaml -b -kK
ansible-playbook -i inventory/openstack.ini openstack.yaml -b
ansible-playbook -i inventory/openstack.ini install-docker.yaml -b

ansible-playbook -i inventory/openstack.ini kolla-ansible-prepare.yaml -b
```

# ==================================================================================================

# K8s1 Redos
```bash
ansible-playbook -i inventory/k8s1-redos.ini general.yaml -b
```

# Test Redos
```bash
ansible-playbook -i inventory/test-redos.ini dns.yaml -b
```

# MAAS
```bash
ansible-playbook -i inventory/maas.ini ping.yaml -b
ansible-playbook -i inventory/maas.ini ssh-keys.yaml -b
ansible-playbook -i inventory/maas.ini general.yaml -b
ansible-playbook -i inventory/maas.ini dns.yaml -b

ansible-playbook -i inventory/maas.ini chrony.yaml -b
ansible-playbook -i inventory/maas.ini timezone.yaml -b
```

# OpenStack
```bash
ansible-playbook -i inventory/openstack.ini general.yaml -b
```

# K8s1-Ubuntu-Lab
```bash
ansible-playbook -i inventory/k8s1-ubuntu-lab.ini general.yaml -b
```

# K8s1-RHEL
```bash
ansible-playbook -i inventory/k8s1-rhel.ini general.yaml -b -kK
ansible-playbook -i inventory/k8s1-rhel.ini ssh-keys.yaml -b -kK
ansible-playbook -i inventory/k8s1-rhel.ini ping.yaml -b
ansible-playbook -i inventory/k8s1-rhel.ini update.yaml -b
```

# Test-keepalived
```bash
ansible-playbook -i inventory/test-keepalived.ini ping.yaml -b
ansible-playbook -i inventory/test-keepalived.ini install-keepalived.yaml -b
```

# Kafka Zookeeper
```bash
ansible-playbook -i inventory/kafka-zoo.ini ping.yaml -b
ansible-playbook -i inventory/kafka-zoo.ini install-kafka-zookeeper.yaml -b
```

# OpenSearch My
```bash
ansible-playbook -i inventory/test-opensearch-cluster-1.yaml ping.yaml -b
ansible-playbook -i inventory/test-opensearch-cluster-1.yaml create-lvm-partition.yaml -b
ansible-playbook -i inventory/test-opensearch-cluster-1.yaml install-opensearch-my.yaml \
    --extra-vars "opensearch_admin_password=7FBEa3J853N2c7U8" -b
```

# OpenSearch Prod Ready
```bash
ansible-playbook -i inventory/test-opensearch-cluster-prod-ready-1.yaml ping.yaml -b
ansible-playbook -i inventory/test-opensearch-cluster-prod-ready-1.yaml create-lvm-partition.yaml -b
ansible-playbook -i inventory/test-opensearch-cluster-prod-ready-1.yaml install-opensearch-prod-ready.yaml \
    --extra-vars "admin_password=myStrongPassword@123! kibanaserver_password=Test@6789 logstash_password=Test@456" -b
```
# ==============================================================================
#                                K8s1 RHEL Linux
# ==============================================================================
ansible-playbook -i inventory/k8s1-rhel.ini ping.yaml -b
ansible-playbook -i inventory/k8s1-rhel.ini update.yaml -b
ansible-playbook -i inventory/k8s1-rhel.ini general.yaml -b
# ==============================================================================
#                                K8s1 Alma Linux
# ==============================================================================

```bash
ansible -i k8s1-alma-vm.yaml all \
    -m setup \
    -u=cloud-user \
    --ssh-common-args="-o StrictHostKeyChecking=no" \
    -b \
    > k8s1-alma-vm-setup.json
```

source .venv/bin/activate
ansible-playbook -i inventory/k8s1-alma.yaml ping.yaml -b
ansible-playbook -i inventory/k8s1-alma.yaml update.yaml -b

ansible-playbook -i inventory/k8s1-alma.yaml general.yaml -b
<!-- 
ansible-playbook -i inventory/k8s1-alma.yaml ssh-keys.yaml -b
ansible-playbook -i inventory/k8s1-alma.yaml passwordauthentication-no.yaml -b
ansible-playbook -i inventory/k8s1-alma.yaml sudoers.yaml -b
-->
# ==============================================================================
#                                K8s2 Alma Linux
# ==============================================================================
ansible-playbook -i inventory/k8s2-alma.yaml ping.yaml -b
ansible-playbook -i inventory/k8s2-alma.yaml update.yaml -b

ansible-playbook -i inventory/k8s2-alma.yaml general.yaml -b
# ==============================================================================
#                              K8s1 Altlinux Linux
# ==============================================================================
ansible-playbook -i inventory/k8s1-altlinux.yaml ping.yaml -b
ansible-playbook -i inventory/k8s1-altlinux.yaml ssh-keys.yaml -b
# ==============================================================================