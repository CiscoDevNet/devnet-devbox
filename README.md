# sandbox-devbox
Documentation around the DevNet Sandbox Devbox VM

# Usage

`vagrant up`

# VM Information

* OS: CentOS 7
* Mem: 2GB
* HD: 20GB


# Software

* Gnome Desktop
* Docker Daemon and Engine
* git tools
* pyenv
* Python 2.7 and 3.5
* pip
* virtualenv
* drone command line tool
* PyCharm Community
* node version manager (nvm)
* node v6.9.2 (LTS)
* ~~atom 1.12.7~~

# Notes

* To run Python 2.7.5, use the command `$ python`.  To run Python 3.5, use the command `$ python3.5`

# Known Issues

* nvm not loading when `devbox` user logs in.  Workaround: `$ source ~/.nvm/nvm.sh`
* No Atom installation yet
* You must restart the VM after Ansible completion to have the gnome desktop load by default

For details on the Ansible playbook view the [README](devbox/README.md)
