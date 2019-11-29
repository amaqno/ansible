# ANSIBLE

### Document Information

- Created by: Am Aqno
- Reviewed by: 
- Capability: Ansible
- Tools: Linux, Ansible

### Version History

| Version | Updated by | Date | Modifications |
|-------|:-------------|:-----|:-----|
| 1.0 - Draft | am aqno | 11/20/2019 | |

## Overview

Contains howto's related to Ansible

### General Information


### Setup pre-requisites 
- Ansible Worksation / ACS

Ansible is setup and configured in an Ubuntu server.


*How to Setup Ansible in Ubuntu*
```
$ sudo apt-get install software-properties-common

$ sudo apt-add-repository ppa:ansible/ansible

$ sudo apt-get update

$ sudo apt-get install ansible

$ sudo apt-get install -y python-pip

$ sudo apt-get install azure-cli

pip install azure

pip install msrestazure

```
### Update configurations
Update the plugins in  /etc/ansible/ansible.cfg

[inventory]
enable_plugins = host_list, virtualbox, yaml, constructed, azure_rm

### Setup Service Principal
Create ~/.azure/credentials with Service Principal user details 
MS https://docs.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli?view=azure-cli-latest


