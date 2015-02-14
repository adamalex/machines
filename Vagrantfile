# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.define "dev" do |config|
    config.vm.provision :shell, path: "machine/dev"
  end

  config.vm.define "dockerfig" do |config|
    config.vm.provision :shell, path: "machine/dockerfig"
  end

  # Uncomment the following line if creating a base box
  # config.vm.provision :shell, path: "script/basebox"
end
