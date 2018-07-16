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

```
Name		Help for feature: jnlp
 	Docker image		Help for feature: openshift/jenkins-slave-base-centos7
 	Always pull image		
 	Working directory		Help for feature: /tmp
 	Command to run		Help for feature: ${computer.jnlpmac} ${computer.name}
 	Arguments to pass to the command		Help for feature: Arguments to pass to the command
 	Allocate pseudo-TTY	
```

Licence
=============
Apache
