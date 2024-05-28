What changes to make:

1. Hosts file contains two groups.
	a. Add worker nodes to both groups accordingly
	b. Check which version of python exists on each node
	c. Check the installation directory of that python version (I used `type python2` or `type python3`)
	d. Copy the path and paste it in the hosts file
2. To install Filebeat on Oracle linux nodes, use this command (update with your command):
ansible-playbook install_filebeat_yum.yml -i hosts -u root
2. To install Filebeat on Ubuntu nodes, use this command (update with your command):
ansible-playbook install_filebeat_apt.yml -i hosts -u root