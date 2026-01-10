# Log into Docker
docker exec -it hadoop-cli bash

# File System commands
hdfs dfs -ls /

# Set Hadoop User
export HADOOP_USER_NAME=root

# Create directory in HDFS
hdfs dfs -mkdir -p /user/hadop/books /user/hadoop/temp /tmp

# List Directories
hdfs dfs -ls /

# Remove folders
hdfs dfs -rm -r /user /tmp


