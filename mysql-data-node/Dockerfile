FROM centos:7
RUN yum install https://dev.mysql.com/get/Downloads/MySQL-Cluster-7.6/mysql-cluster-community-server-7.6.11-1.el7.x86_64.rpm -y && \
yum autoremove -y && yum clean all && rm -rf /var/cache/yum
RUN mkdir -p /opt/mysql-cluster/config /opt/mysql-cluster/data && \
adduser -u 1001 -D mysql && \
chown -R 1001 /opt && chgrp -R 0 /opt && chmod -R g=u /opt 
