# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  ## Escolha da Box
  config.vm.box = "ubuntu/bionic64"

  ## DATABASE
  config.vm.define "databasenew" do |db|
    db.vm.network "private_network", ip: "172.17.177.21"
    db.vm.hostname = "databasenew"

    # Configurações de Size da VM
    db.vm.provider "virtualbox" do |v|
      v.name = "databasenew"
      v.memory = 512
      v.cpus = 2
    end

  end

  ## BLOG
  config.vm.define "blognew" do |blog|
    blog.vm.network "private_network", ip: "172.17.177.22"
    blog.vm.hostname = "blognew"


    # Configurações de Size da VM
    blog.vm.provider "virtualbox" do |v|
      v.name = "blognew"
      v.memory = 512
      v.cpus = 2
    end

  end

  ## CONTROLLER
  config.vm.define 'controllernew' do |controller|
    controller.vm.network "private_network", ip: "172.17.177.11"
    controller.vm.hostname = "controllernew"

    # Configurações de Size da VM
    controller.vm.provider "virtualbox" do |v|
      v.name = "controllernew"
      v.memory = 512
      v.cpus = 2
    end
  end
end