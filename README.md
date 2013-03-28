# Instructions

This script installs/configures nginx to serve a page on http://localhost:8080 across one or more target hosts via [Ansible](http://ansible.cc/).

Tested on Debian/Ubuntu and RHEL/CentOS distributions.

## Prerequisites

Install Ansible via pip and easy_install (requires [distribute/setuptools](https://pypi.python.org/pypi/distribute)):

    # easy_install pip
    # pip install ansible

## Deploying

### Define target hosts

Edit the `hosts` file and add target hostnames (by default `hosts` only contains a single entry `localhost`).

### Run deploy script

Use `./deploy [user]` to run. NOTE: The deploy user specified must exist on the target system and must have sudo capabilities.

