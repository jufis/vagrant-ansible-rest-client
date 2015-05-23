# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "jufis/rawhide"
  config.vm.box_url = "file:///home/jufis/Desktop/sandbox/src/github/vagrant-rawhide-box/virtualbox/rawhide.box"
  config.vm.provider "virtualbox" do |v|
      v.memory = 2048
      v.cpus = 1
  end
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "docker-rest-client.yml"
    ansible.verbose = "vvvv"
  end
end

