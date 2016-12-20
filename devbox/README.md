
# Prep

You must have Vagrant and VirtualBox installed.


# Usage

From your command line, execute 'vagrant up'

To manually run run one of the ansible playbooks:

`ansible-playbook -i provision/devbox provision/devbox.yml`

Add `--check --ask-sudo-pass` if you want to run a check or if you need to provide a password for sudo
