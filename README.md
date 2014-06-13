Hadoop ansible-playbooks
=========================

Installs and configure Hadoop system in a cluster of nodes.
How to use it:

In the "Worker Nodes"
```yml
  roles:
    - { role: 'hadoop', hadoop_master: '<MASTER_NODE_NAME_OR_IP>' }
```

In the "Manager Node"
```yml
  roles:
    - { role: 'hadoop', hadoop_master: '<MASTER_NODE_NAME_OR_IP>', hadoop_type_of_node: 'master'}
```
