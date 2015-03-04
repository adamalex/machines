# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.define "devbackend" do |config|
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 2
    end

    config.vm.provision :shell, path: "machine/devbackend"
  end

  config.vm.define "dockercompose" do |config|
    config.vm.provision :shell, path: "machine/dockercompose"
  end

  # Uncomment the following line if creating a base box
  # config.vm.provision :shell, path: "script/basebox"
end
