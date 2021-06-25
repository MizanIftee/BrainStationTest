#Vagrant Installation
Need to install VirtualBox and vagrant.

Please check if vagrant command is working or not by running this command
vagrant --version

After that Create vagrant file for Master and Two Nodes.
Please go to Master and then run below command:
vagrant up

it takes time if Master is setup then node will take less time.
After installing centOS, please run below command:

vagrant ssh

it will take you with login with 'vagrant' user.
please set the root password with 

sudo passwd root

after that please login with root and you are using VM with Root
su root