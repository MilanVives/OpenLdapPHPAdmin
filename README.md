Containers runnen:
```bash
docker-compose up
```
Terminal krijgen op ldap container:
```bash
docker-compose exec ldap /bin/bash 
```
Users zoeken in ldap directory:
```bash
ldapsearch -x -h localhost -b dc=ldap,dc=vives,dc=be -D "cn=admin,dc=ldap,dc=vives,dc=be" -w ldap
```


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


PhpLdapAdmin in webbrowser openen op host:

https://localhost:6443  
login:  cn=admin,dc=ldap,dc=vives,dc=be
psw:      ldap








