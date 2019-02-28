---
title: Prerequisites
workshops: ansible_windows_addon
workshop_weight: 10
layout: lab
---

# Getting Started

This workshop makes the following assumptions:

- Ansible engine is already setup on an Ansible host
- Needed prerequistites as defined on
https://docs.ansible.com/ansible/latest/user_guide/windows.html have
been met for both the Ansible Host and the Windows host we will be
oeprating against. 
    - If needed - the gist of the configuration is: 
        - install WinRM on the windows host as mentioned here: https://docs.ansible.com/ansible/latest/user_guide/windows_setup.html#winrm-setup
        - Ansible uses the pywinrm package to communicate with Windows servers
        over WinRM. It is not installed by default with the Ansible package, but
        can be installed by running the following:
        ```
        pip install "pywinrm>=0.3.0"
        ```



## The Good News

if you dont have an Ansible host setup already, you could use a docker
container that is prepackaged to run this workshop. (note: docker must
installed and functional)
```
docker run -ti williamyeh/ansible:centos7 bash
```
