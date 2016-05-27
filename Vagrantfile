# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define 'TestVM' do |machine|
  machine.vm.box = "centos6.4"

  machine.vm.synced_folder "..", "/share/ansible"
  machine.vm.hostname = "TestVM"
  machine.vm.network "private_network", ip: "192.168.33.20"
  end
end
