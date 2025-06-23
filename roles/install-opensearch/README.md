inventory:

```bash
test-opensearch-cm-1   ansible_host=192.168.2.150  opensearch_node_roles=" cluster_manager "
test-opensearch-d-1    ansible_host=192.168.2.151  opensearch_node_roles=" data, ingest "
test-opensearch-d-2    ansible_host=192.168.2.152  opensearch_node_roles=" data, ingest "
test-opensearch-d-3    ansible_host=192.168.2.153  opensearch_node_roles=" data, ingest "
test-opensearch-c-1    ansible_host=192.168.2.155  opensearch_node_roles=""
```