

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
