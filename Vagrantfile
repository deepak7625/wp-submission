# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.box = "generic-VAGRANTSLASH-ubuntu2004"
  
  #mount shared folder
  config.vm.synced_folder ".", "/opt";
  
  #network configuration
  
  config.vm.network "public_network", bridge: "Intel(R) Wireless-AC 9462"
  
  #provision command
  
  config.vm.provision "shell", path: "bootstrap.sh"

end
