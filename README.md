# ansible-infrastructure
ansible infrastructure scripts for side projects

## Prerequisites
* [Ansible](https://www.ansible.com/) (Tested on v2.7.0)
* [Github API Token](https://github.com/settings/tokens) (For secure repo cloning - Token needs private repo access if applicable and write:public_key access)

### Installation

* Clone down the repository.
```
git clone https://github.com/cynical89/ansible-infrastructure.git
```

* Navigate inside the ansible-infrastructure folder.
```
cd ansible-infrastructure
```

* Edit your config. There are several variables at the top of the yml files with the text `CHANGEME` by them. Replace with your own values.

* Make sure your remote host has your ssh key copied to it
```
ssh-copy-id root@ip
Example : ssh-copy-id root@192.168.1.100
```

* Start it up.
```
ansible-playbook -i ip, ./folder/flavor.yml
Example : ansible-playbook -i 192.168.1.100, ./Centos7/node-redis-couch.yml
```

* Enjoy!
