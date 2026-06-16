# Ansible User Management Automation

## Overview

This project automates Linux user administration using Ansible Roles.

## Features

* Create Linux groups
* Create multiple users
* Assign users to groups
* Configure sudo access
* Role-based project structure

## Environment

* Control Node: CentOS Stream 9
* Managed Nodes: 2 CentOS Stream 9 Servers
* Ansible Core 2.14

## Project Structure

.
├── inventory
├── playbooks
└── roles
└── user_management

## Users Created

* devops
* monitoring
* automation

## Group Created

* admins

## Run Playbook

ansible-playbook -i inventory/hosts playbooks/site.yml

## Verification

id devops
id monitoring
id automation

cat /etc/sudoers.d/admins
