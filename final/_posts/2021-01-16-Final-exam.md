---
layout: post
title:  "Hands-on Final Exam"
date: 2021-01-19 04:06:00 +08:00
categories: final-exam
---
![image](https://user-images.githubusercontent.com/75426228/105005498-60b14780-5a70-11eb-9e53-1bff84ed54eb.png)
# Procedure
1. Fork this repository [https://github.com/ajcanlas-tip/sysad2-12021.git](https://github.com/ajcanlas-tip/sysad2-12021.git) (Links to an external site.)

2. Clone your new repository in your VM https://github.com/< your username >/sysad2-12021.git

3. Create a branch named "final-exam" and checkout in that branch. 

4. Create an Ansible playbook that does the following with an input of a config.yaml file and structure inventory file.

    4.1 Clone your prelim exam repository

    4.2 Install and configure one enterprise service that can be installed in Debian,Centos and OpenSuse servers

    4.3 Install and configure one monitoring tool that can be installed in Debian, Centos and OpenSuse servers (if it is a stack there should be option of different host)

    4.4 Change Motd as "Ansible Managed by <username>"

5. push and commit your final-exam branch in the VM (no need for ansible.cfg upon pushing)

6. request a pull request from that branch in GitHub

7. For your final exam to be counted, please paste your repository link as an answer in this exam.

Note: Extra points if you will implement the said services via containerization.

## Output
[https://github.com/ejvillareal-tip/sysad2-12021/tree/final-exam](https://github.com/ejvillareal-tip/sysad2-12021/tree/final-exam)
```
sysad2-12021
├── 1811401
│   └── final-exam
│       ├── README.md
│       ├── ansible.cfg
│       ├── config.yaml
│       ├── config_files
│       │   ├── ervie_centos.com.conf
│       │   ├── ervie_debian.com.conf
│       │   ├── ervie_opensuse.com.conf
│       │   ├── index.html
│       │   ├── index_centos.html
│       │   ├── index_debian.html
│       │   ├── index_docker.html
│       │   ├── index_opensuse.html
│       │   └── logstash.conf
│       ├── inventory
│       └── roles
│           ├── apache2_debian
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── apache2_opensuse
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── git_clone
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── httpd_centos
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install-ElasticStack-docker
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── files
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── templates
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install-docker-centos
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── files
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── templates
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install-docker-debian
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── files
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── templates
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install-docker-opensuse
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── files
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── templates
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install-httpd-docker
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── files
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── templates
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install_git_centos
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install_git_debian
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── install_git_opensuse
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── motd
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── nagios_centos
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           ├── nagios_debian
│           │   ├── README.md
│           │   ├── defaults
│           │   │   └── main.yml
│           │   ├── handlers
│           │   │   └── main.yml
│           │   ├── meta
│           │   │   └── main.yml
│           │   ├── tasks
│           │   │   └── main.yml
│           │   ├── tests
│           │   │   ├── inventory
│           │   │   └── test.yml
│           │   └── vars
│           │       └── main.yml
│           └── nagios_opensuse
│               ├── README.md
│               ├── defaults
│               │   └── main.yml
│               ├── handlers
│               │   └── main.yml
│               ├── meta
│               │   └── main.yml
│               ├── tasks
│               │   └── main.yml
│               ├── tests
│               │   ├── inventory
│               │   └── test.yml
│               └── vars
│                   └── main.yml
└── README.md
```