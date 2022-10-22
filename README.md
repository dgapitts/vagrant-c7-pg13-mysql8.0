# vagrant-c7-pg13-mysql8.0 - vagrant multi node pg13 cluster with primary-replica replication


## First - manually adding mysql along side pg13 on db1 

Manually I ran these commands

```
wget https://dev.mysql.com/get/Downloads/MySQL-8.0/mysql-8.0.15-1.el7.x86_64.rpm-bundle.tar
tar -xvf mysql-8.0.15-1.el7.x86_64.rpm-bundle.tar
yum -y install perl net-tools
rpm -Uvh mysql-community-{server,client,common,libs}-*
grep 'temporary password' /var/log/mysqld.log
```

and then reset the password manually


```
mysql -u root -p 
ALTER USER 'root'@'localhost' IDENTIFIED BY ..;
```



