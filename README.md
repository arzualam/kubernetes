# kubernetes Secrets
## How to add a certificate to kubernetes with ansible by using kubernetes Module. 

Certificates can be managed in 2 ways, first and most desired way is to create a secret from the certificate file and add it as volume to the containers. Here I am  providing the sniphet for a deployment file with ansible.

Refer to the kubernetes-secrets.yaml file.

## How to add a file ( in my case a pemfile from your local folder to kubernetes pods with ansible)

To move a file inside a container during the deployment, or container starting process, can be attached as volume with the help of configMap.

First we download the file in local with ansible, then we create a configMap, after that attach the configMap as volume in the deployment kind

refer to kubernetes-configmap.yaml

