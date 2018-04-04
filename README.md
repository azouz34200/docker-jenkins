Introduction
=============

This docker-compose file permit to create jenkins master with nginx proxy

Usage
=============

```
docker-compose up -d
```

In your webroswer do : http://localhost/

Openshift
============

```
oc create serviceaccount jenkins_oc
oc policy add-role-to-user edit -z jenkins-oc -n ci
oc serviceaccounts get-token jenkins-oc -n ci
```


Licence
=============
Apache
