
# Software Requirements

Tested on Vagrant 1.9.1, Ansible 2.1.1.0 and VirtualBox 5.0.30.

# Usage

Review and configure variables contained in `devbox/provision/group_vars`

From within this project, execute 'vagrant up'

On my workstation and home bandwidth, it takes about 12 minutes to complete the playbook.

# Profile
```
Wednesday 21 December 2016  22:52:34 -0700 (0:00:00.731)       0:12:13.622 ****
===============================================================================
python : install python versions into $PYENV_ROOT/versions ------------ 156.22s
common : Install gnome minimal ---------------------------------------- 136.83s
python : install python versions into $PYENV_ROOT/versions ------------ 116.58s
pycharm : download ----------------------------------------------------- 99.81s
common : install the 'Development tools' package group ----------------- 63.30s
common : waiting for server to come back ------------------------------- 40.49s
common : install the 'XWindows' environment group ---------------------- 22.21s
common : Install dependencies ------------------------------------------ 20.36s
docker : install packages ---------------------------------------------- 16.71s
pycharm : install ------------------------------------------------------ 13.01s
node : install nodejs using nvm ----------------------------------------- 4.73s
node : Install nvm ------------------------------------------------------ 3.65s
drone-cli : unpack drone ------------------------------------------------ 3.64s
python : pyenv | install devel packages --------------------------------- 3.24s
setup ------------------------------------------------------------------- 2.35s
docker : start docker --------------------------------------------------- 2.09s
python : virtualenv install --------------------------------------------- 2.08s
python : pyenv | update pyenv repo -------------------------------------- 1.96s
common : restart machine ------------------------------------------------ 1.30s
users : add user -------------------------------------------------------- 1.28s
```

# Manually run playbook

(Not tested)

To manually run the ansible playbook:

`ansible-playbook -i provision/devbox provision/devbox.yml`

Add `--check --ask-sudo-pass` if you want to run a check or if you need to provide a password for sudo
