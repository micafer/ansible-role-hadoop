Hadoop ansible role
=========================

Installs and configure Hadoop system (version 1.2.1) in a cluster of nodes.
How to use it:

In the "Worker Nodes"
```yml
  roles:
    - { role: 'micafer.hadoop', hadoop_master: 'MASTER_NODE_NAME_OR_IP' }
```

In the "Manager Node"
```yml
  roles:
    - { role: 'micafer.hadoop', hadoop_master: 'MASTER_NODE_NAME_OR_IP', hadoop_type_of_node: 'master'}
```
