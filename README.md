docker-compose up

docker-compose exec ldap /bin/bash 

ldapsearch -x -h localhost -b dc=ldap,dc=vives,dc=com -D "cn=admin,dc=ldap,dc=vives,dc=com" -w vives


<pre>
# extended LDIF
#
# LDAPv3
# base <dc=example,dc=org> with scope subtree
# filter: (objectclass=*)
# requesting: ALL
#

[...]

# numResponses: 3
# numEntries: 2
</pre>

https://localhost:6443  
login:  cn=admin,dc=ldap,dc=vives,dc=be
psw:      ldap








