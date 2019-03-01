# Learning HashiCorp Vault
This project is to assist to learn HashiCorp Vault to manage secrets and encryption in a Multi-Cloud environment.  This is my own hands-on outcome of learning Vault.

Make sure that you have installed the latest version of VirtualBox and Vagrant in your laptop.

## Installation
Simply clone this repository and change direcvtory to the cloned folder. Then build the vagrant environment as follows:


``` bash
$git clone https://github.com/sharabinth/Learning-Hashicorp-Vault.git
$cd Learning-Hashicorp-Vault
$vagrant up
```

This takes about 3 to 10 minutes to complete on a MacBook Pro depedning on the download speed. This will build a Dev Vault cluster along with a single node Consul.

## Validate Vault Cluster

Vault UI http://192.168.50.152:8200/

Initially login with the root VAULT_TOKEN.

Consul UI http://192.168.50.152:8500/


Once setup, use 
``` bash
$vagrant ssh
```
to loginto the VM to view the Dev Vault cluster.

VAULT_TOKEN environment variable is already set for this cluster.

``` bash
$echo VAULT_TOKEN
```

Check the Vault and Consul instances

``` bash
$ps -ef | grep vault
....
$ps -ef | grep consul
```



