Prerequisites
=============
Once you have easy_install, make sure Ansible is installed with pip:

    # easy_install pip
    # pip install ansible

Deploying
=========
Edit the `hosts` file and add target hostnames (by default `hosts` only contains a single `localhost` entry).

You can deploy by running:

    $ ./deploy [user]

The deploy user specified above must exist on the target system and must have sudo capabilities to run.
