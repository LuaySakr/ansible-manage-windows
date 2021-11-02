Setps
Windows machine

add new local admin user
log in to this local user
install python 3


ubuntu machine 
sudo apt update
sudo apt install ansible
ansible-galaxy collection install ansible.windows

sudo nano /etc/ansible/hosts


[win]
10.0.2.7
[win:vars]
ansible_user=ansibleuser1
ansible_password=password
ansible_port=5986
ansible_connection=winrm
ansible_winrm_server_cert_validation=ignore

