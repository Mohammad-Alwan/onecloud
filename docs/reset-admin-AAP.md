---
date: '2026-01-01'
---
# Reset Admin user password for Ansible Automation Platform

## Login to Hub server
Log in to the Automation Hub Server if using a cluster installation.

## Steps to reset the Admin 
```
$ sudo su -
# export PULP_SETTINGS=/etc/pulp/settings.py
# pulpcore-manager reset-admin-password
Please enter new password for user "admin": 
Please enter new password for user "admin" again: 
Successfully set password for "admin" user.
# exit
```