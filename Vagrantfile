# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
    config.vm.box = "bento/ubuntu-22.04"
    config.vm.provision "dev", type: "shell", inline: <<-SHELL
    sudo apt-get update
    # dev tools
    sudo apt-get install -y git cmake htop binutils build-essential pkg-config
    SHELL
        #set the shared folder
    config.vm.synced_folder "workspace", "/home/vagrant/workspace"

  end