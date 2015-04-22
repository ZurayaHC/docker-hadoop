# docker-hadoop
Hadoop

```{bash}
docker run -ti --rm \
  -e "AUTHORIZED_SSH_PUBLIC_KEY=$(cat ~/.ssh/id_rsa.pub)" \
  -v /home/nano/tmp/docker-hadoop-data/:/home/hduser/hdfs-data/ \
  -v /home/nano/tmp/docker-hadoop-logs/:/srv/hadoop/logs/ \
  -p 2122:2122 -p 2181:2181 -p 39534:39534 -p 9000:9000 \
  -p 50070:50070 -p 50010:50010 -p 50020:50020 -p 50075:50075 \
  -p 50090:50090 -p 8030:8030 -p 8031:8031 -p 8032:8032 \
  -p 8033:8033 -p 8088:8088 -p 8040:8040 -p 8042:8042 \
  -p 13562:13562 -p 47784:47784 -p 10020:10020 -p 19888:19888 \
hadoop_pseudo /bin/bash
```
