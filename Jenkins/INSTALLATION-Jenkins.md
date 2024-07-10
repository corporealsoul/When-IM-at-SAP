### Manage Repo
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git config --global user.email "bca.anup@gmail.com"
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git config --global user.name "Anup Kumar Mondal"

[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git add .
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git status
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git commit -m "When-IM-at-SAP-Jenkins"
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git status
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git push
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ git branch

### Installation
https://www.jenkins.io/doc/book/installing/linux/#red-hat-centos

[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo systemctl enable jenkins
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo systemctl start jenkins
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo systemctl status jenkins

http://192.168.56.102:8080/

[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo cat /var/lib/jenkins/secrets/initialAdminPassword

[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo systemctl status firewalld.service
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo firewall-cmd --zone=public --add-port=8080/tcp 
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo firewall-cmd --reload
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo firewall-cmd --zone=public --list-ports

### Run shell command with Sudo
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo visudo
root    ALL=(ALL)       ALL
anup    ALL=(ALL)       ALL
jenkins ALL=(ALL)       NOPASSWD:ALL
