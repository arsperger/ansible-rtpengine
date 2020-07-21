# About

Ansible role to setup and configure [rtpengine](https://github.com/sipwise/rtpengine) on Debian 10 (Buster)

Role will install all prerequisites. 
Tested on AWS Debian 10 VMs. 
Configuration suppose that the server is listening on local IP (advertised IP has to be set) 

To install role create a file with:
```
- hosts: voiptest1
  import_role:
     - name: rtpengine
```

### Note
libbcg729 deb have been pre-built. To make it easier rtpengine pre-built packages could be also placed there :)

Ansible 2.9
