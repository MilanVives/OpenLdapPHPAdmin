docker-compose up

docker-compose exec ldap /bin/bash 

ldapsearch -x -h localhost -b dc=ldap,dc=vivesdata,dc=com -D "cn=admin,dc=ldap,dc=vivesdata,dc=com" -w vives


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



ldapsearch -x -h localhost -b dc=ldap,dc=vivesdata,dc=com -D "cn=screwyou,dc=ldap,dc=vivesdata,dc=com" -w screwyou "(&(objectClass=posixAccount)(uid=testldap))"




