# Linux Infrastructure Deployment & Hardening Lab

## Overview

This project demonstrates the deployment, administration, and hardening of a Linux server environment using core system administration skills. The lab simulates a small company infrastructure where users, groups, permissions, web services, firewall rules, and troubleshooting procedures are configured and managed.

The project was built as part of a hands-on Linux System Administration learning path and combines multiple administrative tasks into a single real-world environment.


## Objectives

* Configure Linux hosts and verify network connectivity
* Implement SSH-based remote administration
* Manage users and groups
* Configure file permissions and ownership
* Implement Access Control Lists (ACLs)
* Deploy and manage Apache HTTP Server
* Monitor and manage system processes
* Install and manage software packages
* Configure and secure the firewall using Firewalld
* Troubleshoot service failures using system logs
* Document incidents and administrative procedures


## Environment

### Server Roles

| Server  | Purpose                           |
| ------- | --------------------------------- |
| admin01 | Administrative workstation        |
| web01   | Apache web server                 |
| file01  | File and access management server |

### Operating System

* RHEL-based Linux Distribution

## Project Components

### User and Group Management

Created departmental users and groups to simulate a company environment.

Tasks performed:

* User creation
* Group creation
* Password management
* User-group assignment

Commands used:

useradd
groupadd
usermod
passwd

### Permissions Management

Configured secure access to departmental directories using standard Linux permissions.

Tasks performed:

* Ownership management
* Permission assignment
* Shared directory configuration

Commands used:

chmod
chown
umask

### Access Control Lists (ACLs)

Implemented fine-grained access control without changing ownership or primary groups.

Tasks performed:

* ACL creation
* ACL verification
* Special user access assignment

Commands used:

setfacl
getfacl

### SSH Administration

Configured secure remote access and passwordless authentication.

Tasks performed:

* SSH key generation
* Key deployment
* Remote login testing

Commands used:

ssh
ssh-keygen
ssh-copy-id

### Apache Web Server Deployment

Installed and configured Apache HTTP Server.

Tasks performed:

* Package installation
* Service management
* Custom web page deployment
* Service verification

Commands used:

dnf
systemctl
httpd

### Process Management

Monitored and managed running system processes.

Tasks performed:

* Process inspection
* Process termination
* Resource monitoring

Commands used:

ps
top
kill
pkill

### Log Analysis and Troubleshooting

Investigated and resolved service failures using system logs.

Tasks performed:

* Log inspection
* Apache troubleshooting
* Service recovery

Commands used:

journalctl
journalctl -xe
journalctl -u httpd

### Package Management

Installed, updated, and removed software packages.

Commands used:

dnf
rpm

### Firewall Configuration

Configured firewall rules to secure the server while allowing web traffic.

Tasks performed:

* HTTP access configuration
* HTTPS access configuration
* Firewall verification

Commands used:

firewall-cmd

## Directory Structure

Linux-Infrastructure-Deployment-Lab/
│
├── README.md
├── scripts/
│   ├── user_setup.sh
│   ├── permission_setup.sh
│   ├── acl_setup.sh
│   ├── apache_deploy.sh
│   ├── firewall_setup.sh
│   └── process_monitor.sh
│
├── docs/
│   ├── network_configuration.md
│   ├── ssh_setup.md
│   ├── troubleshooting_report.md
│   └── incident_report.md
│
├── screenshots/
│   ├── users_created.png
│   ├── acl_configured.png
│   ├── apache_running.png
│   ├── firewall_rules.png
│   └── website_access.png
│
└── reports/
    └── process_report.txt

## Skills Demonstrated

* Linux System Administration
* User and Group Management
* File Permissions and ACLs
* SSH Administration
* Apache Web Server Deployment
* Process Monitoring
* Package Management
* Firewall Administration
* Service Troubleshooting
* Technical Documentation

## Key Learning Outcomes

Through this project, I gained practical experience in deploying and managing Linux infrastructure, securing system resources, configuring network services, troubleshooting operational issues, and documenting administrative procedures using industry-standard Linux tools.

## Author

Nandana Mohan J
