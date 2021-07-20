Quick template to deploy clc on Openshift v4

To use it, you need the openshift client (oc), and enough access to 
a project/namespace on your openshift cluster.

The template can be deployed with this command: 
```
oc process -p APPLICATION_DOMAIN=clc.example.org -p ADMIN_PASSWORD=s3cr3t  -f clc.yml | oc create -f - 
oc start-build clc
```
