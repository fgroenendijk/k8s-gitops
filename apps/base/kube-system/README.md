# kube-system namespace

## Authentication

Proxy for the Kubenernetes nginx so I can authenticate users with Open ID.

[Settings](authentication)

## Common Internet File System - CIFS (smb / Samba)

Install tools that allow mounting [CIFS](https://en.wikipedia.org/wiki/Server_Message_Block) volumes.

[Settings](cifs.yaml)

## Kubernetes dashboard settings

Configures the [Kubernetes dashboard](https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/).

** NOTE **: this is not the dashboard but only the settings. The installation is done as part of installing the K8S cluster.

[Settings](dashboard.yaml)

## Gluster

Cluster file system using [gluster](https://www.gluster.org/) and [Heketi](https://github.com/heketi/heketi) to dynamically provide volumes.

TBD: since Heketi is in maintenance mode I need to move to another solution.

[Settings](glusterfs)

## Mail server - Exim

Mail server with [Exim](https://www.exim.org/) for application in K8S and LAN to send mail without having to store any Google settings.

[Settings](mailserver.yaml)

## Metallb - Load Balancer

[Load balancers](https://metallb.universe.tf/) for K8S services.

[Settings](metallb.yaml)

## NFS

Some [Persistant Volume Claims](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistentvolumeclaims) for the NAS.

[Settings](nfs)

## Others (to be moved)

  * [cert-manager](https://github.com/jetstack/cert-manager) - Automated letsencrypt broker