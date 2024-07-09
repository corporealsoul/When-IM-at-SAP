### Manage Repo

[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git config --global user.email "bca.anup@gmail.com"
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git config --global user.name "Anup Kumar Mondal"

[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git add .
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git status
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git commit -m "When-IM-at-SAP-Jenkins"
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git status
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git push
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ git branch

### Installation
https://www.jenkins.io/doc/book/installing/linux/#red-hat-centos

[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo systemctl status firewalld.service
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo firewall-cmd --zone=public --add-port=8080/tcp 
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo firewall-cmd --reload
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo firewall-cmd --zone=public --list-ports

[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo systemctl enable jenkins
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo systemctl start jenkins
[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo systemctl status jenkins

http://192.168.56.101:8080/

[anup@infrastructure-management-and-provisioning When-IM-at-SAP]$ sudo cat /var/lib/jenkins/secrets/initialAdminPassword
