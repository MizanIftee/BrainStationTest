# Ansible Playbook Conf for Kubernetes
First install ansible from control server

**How to configure password less conf in master nodes and worker nodes**
From Master server run
> ssh-keygen
copy the content *id_rsa.pub* from ~/.ssh/
Go To the worker node and run *ssh-keygen*.
after that paste the content of public key of master server in worker nodes.
Go to ~/.ssh/ and create *authorized_keys* and paste there the contents.

1st time need to give password and after that it will be password less ssh login.

**Ansible conf and Playbook**
Please go *ansible.cfg* and comment out *inventory      = /etc/ansible/hosts*
then got to *hosts* file add the master and worked node in like below:
>[anyname]
>hostname ansible_host=192.168.1.3

Please check after adding if all nodes could be login by ansisble through below commands:
>ansible -m ping all
it will give you success message

Now Run below ymls to configure Cluster

Before that you could check if your syntax is OK or not
>ansible-playbook serverprep.yml --syntax-check

Run below yml for Server Preparation:
>ansible-playbook serverprep.yml

After Preparing the server, run below to configure the Masternode:
>ansible-playbook masternodeconf.yml

After getting the master node ready need to prepare the Worker node:
>ansible-playbook workernodeconf.yml

To get the Dashboard, Metric Server and Service Account With Rbac:
>ansible-playbook dashboard_metricserver_svcrbac.yml
