# HDFS_replication

HDFS can partition large files into blocks to share the storage across many workers, and it can replicate those blocks so that data is not lost even if some workers die.

In this project, we deployed a small HDFS cluster and uploaded a large file to it, with different replication settings. We've written Python code to read the file. When data is partially lost (due to a node failing), our code will recover as much data as possible from the damaged file.

Learning objectives:

use the HDFS command line client to upload files;

use the webhdfs API (https://hadoop.apache.org/docs/r1.0.4/webhdfs.html) to read files;

measure the impact buffering has on read performance;

relate replication count to space efficiency and fault tolerance
