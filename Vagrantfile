# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "centos71"

  config.vm.network "private_network", ip: "10.10.11.14"
  config.vm.network "forwarded_port", guest: 80, host: 80

  config.vm.synced_folder ".", "/data/www/provision"
end
