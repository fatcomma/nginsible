## Overview

This script installs/configures nginx to serve a page on http://localhost:8080 across one or more target hosts via [Ansible](http://ansible.cc/).

Tested on Debian/Ubuntu and RHEL/CentOS distributions.

## Prerequisites

Before deploying you'll need to install Ansible through [pip](https://pypi.python.org/pypi/pip):

    # pip install ansible

You can also install through [distribute/setuptools](https://pypi.python.org/pypi/distribute):
  
    # easy_install ansible

## Usage

### Define target hosts

First, edit the `hosts` file and add target hostnames (by default `hosts` only contains a single entry `localhost`). These can be in the form of domains (web.example.com) or IP addresses (192.168.0.1). 

For details see Ansible's documentation on [Hosts and Groups](http://ansible.cc/docs/patterns.html#hosts-and-groups).

### Run deploy script

NOTE: The deploy user specified must exist on the target system and must have sudo capabilities.

Once the target hosts have been defined use `./deploy [user]` to run.  


