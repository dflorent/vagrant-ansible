# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "ansible/playbook.yml"
  end

  config.vm.hostname = 'vagrant-ansible.dev'
  config.hostmanager.enabled = true
  config.hostmanager.manage_host = true
end
