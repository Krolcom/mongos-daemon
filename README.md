mongos-daemon
=============

centos rhel5 mongos daemon

```
#cd /etc/
#wget https://raw.github.com/Krolcom/mongos-daemon/master/mongos
#cd /etc/init.d/
#wget https://raw.github.com/Krolcom/mongos-daemon/master/mongos.conf
#chmod 755 /etc/mongos.conf
#touch /path/to/log.log
#chown mongod:mongod /path/to/log.log

configure /etc/mongos.conf to have your settings
configure /etc/init.d/mongos to have your settings

#/etc/init.d/mongos start
```

logroll
-------
Add the following to a crontab:
```
1 0 * * * /etc/init.d/log-roll
```
