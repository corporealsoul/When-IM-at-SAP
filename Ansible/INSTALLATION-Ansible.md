### Ansible Installation
[anup@automation-and-continuous-delivery Jenkins]$ sudo yum update
[anup@automation-and-continuous-delivery Jenkins]$ sudo yum install epel-release
[anup@automation-and-continuous-delivery Jenkins]$ sudo yum install ansible
[anup@automation-and-continuous-delivery Jenkins]$ ansible --version

[anup@automation-and-continuous-delivery playbooks]$ sudo useradd ansible
[anup@automation-and-continuous-delivery playbooks]$ sudo passwd ansible
[anup@automation-and-continuous-delivery playbooks]$ sudo usermod -aG wheel ansible

[anup@automation-and-continuous-delivery playbooks]$ sudo su -s /bin/bash jenkins

[anup@automation-and-continuous-delivery playbooks]$ sudo su - ansible
[ansible@automation-and-continuous-delivery ~]$ ssh-keygen -t rsa -b 2048
[ansible@automation-and-continuous-delivery ~]$ ssh-copy-id ansible@192.168.56.101

[ansible@automation-and-continuous-delivery ~]$ ansible all -m ping

[ansible@automation-and-continuous-delivery ~]$ ansible-playbook /etc/ansible/playbooks/gather_facts.yml -f 5