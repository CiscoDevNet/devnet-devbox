VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "centos/7"

  config.vm.provider "virtualbox" do |v|
    v.gui = true
    v.memory = 2048
  end

  config.vm.provision "ansible" do |ansible|
    ansible.groups = {
      "devbox" => ["default"]
    }
    ansible.config_file = "devbox/ansible.cfg"
    ansible.verbose = "v"
    ansible.playbook = "devbox/provision/devbox.yml"
    #ansible.tags = "pycharm"
  end
end
