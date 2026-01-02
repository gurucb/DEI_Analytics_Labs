# Lab 1:

### Create ZK Cluster
docker compose up -d zookeeper

### Build HDFS Name Node
docker compose up -d namenode

### Build HDFS Data Nodes
docker compose up -d datanode1 
docker compose up -d datanode2

### Build YARN Cluster
docker compose up -d resourcemanager nodemanager1 historyserver

### Build hadoop-cli node to interact with Hadoop Cluster
docker compose up -d hadoop-cli

### Test URLS to see if Hadoop nodes are functional.

NameNode: http://localhost:9870
DataNode1: http://localhost:9864
DataNode2: http://localhost:9865
ResourceManager: http://localhost:8088
NodeManager: http://localhost:8042
JobHistory: http://localhost:8188