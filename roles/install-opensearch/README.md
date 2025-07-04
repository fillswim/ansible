# Inventory

## test-opensearch-cluster-1.yaml

inventory/test-opensearch-cluster-1.yaml:

```yaml
test_opensearch_cluster_1:
  children:
    os_cluster:
    # dashboards:

os_cluster:
  children:
    master:
    data:

master:
  hosts:
    opensearch-master-1:
      ansible_host: 192.168.2.151
      roles: cluster_manager
    opensearch-master-2:
      ansible_host: 192.168.2.152
      roles: cluster_manager
    opensearch-master-3:
      ansible_host: 192.168.2.153
      roles: cluster_manager

data:
  hosts:
    opensearch-data-1:
      ansible_host: 192.168.2.154
      roles: data,ingest
    opensearch-data-2:
      ansible_host: 192.168.2.155
      roles: data,ingest
    opensearch-data-3:
      ansible_host: 192.168.2.156
      roles: data,ingest
```

# Group vars

## test_opensearch_cluster_1.yml

group_vars/test_opensearch_cluster_1.yml:

```yaml
# =========================================================================
#                       Install cluster OpenSearch
# =========================================================================
# Cluster settings
opensearch_cluster_name: "test-opensearch-cluster"
opensearch_all_nodes_inventory_group_name: "os_cluster"
opensearch_masters_inventory_group_name: "master"
# Data and logs settings
opensearch_data_folder: "/var/lib/opensearch"
opensearch_logs_folder: "/var/log/opensearch"
# =========================================================================
```

# Установка

```bash
ansible-playbook -i inventory/test-opensearch-cluster-1.yaml install-opensearch.yaml \
    --extra-vars "opensearch_admin_password=7FBEa3J853N2c7U8" -b
```