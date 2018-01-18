

Create a new user (10 is the userid and maas is the name):
$ sudo ./dcmitool user set name 10 maas

Set password for the new user:
$ sudo ./dcmitool user set password 10 <password_here>

Identifying channel id (look for LAN):
$ sudo ./dcmitool channel info 1

Make new user ADMINISTRATOR
$ sudo ./dcmitool channel setaccess 1 10 callin=on ipmi=on link=on privilege=4

List users:
$ sudo ./dcmitool user list 1

Problem: can't disable/downgrade privelege fro the user 15 with name 'USERID'.

Ubuntu 14.04.2 kernel (3.16) has to be < 3.19
# Links:
## OpenCompute IPMI:
 1. https://wiki.ubuntu.com/OpenCompute
 2. https://bugs.launchpad.net/opencompute/+bug/1156667
 3. https://launchpad.net/~opencompute-developers/+archive/ubuntu/ocp-certification-tools-ppa
 4. https://gist.github.com/borislavm/e15079dccacf0af3b77a740f993ce872
## MAAS
 1. https://insights.ubuntu.com/2016/01/23/maas-setup-deploying-openstack-on-maas-1-9-with-juju/
 2. https://paste.ubuntu.com/14567573/
