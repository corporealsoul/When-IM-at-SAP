### Installation
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo yum install httpd

[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo systemctl status httpd.service
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo systemctl start httpd.service
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo systemctl enable httpd.service

[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo firewall-cmd --zone=public --add-port=80/tcp --permanent
[anup@automation-and-continuous-delivery When-IM-at-SAP]$ sudo firewall-cmd --reload

[anup@automation-and-continuous-delivery html]$ sudo wget https://github.com/themewagon/dashdarkX/releases/download/v1.0.0/dashdarkx-v1.0.0.zip

[anup@automation-and-continuous-delivery html]$ sudo wget https://github.com/technext/sneat/archive/refs/tags/v1.0.0.zip
[anup@automation-and-continuous-delivery html]$ sudo unzip v1.0.0.zip