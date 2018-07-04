# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "loadbalancer" do |app|
    app.vm.box = "bento/ubuntu-16.04"
    app.vm.network "private_network", ip: "192.168.33.11"
    app.vm.hostname = "loadbalancer"
    app.vm.provider "virtualbox" do |v|
        v.memory = 512
        v.cpus = 1
      end
    end
  config.vm.define "webserver-one" do |app|
    app.vm.box = "bento/ubuntu-16.04"
    app.vm.network "private_network", ip: "192.168.33.12"
    app.vm.hostname = "webserver-one"
    app.vm.provider "virtualbox" do |v|
        v.memory = 512
        v.cpus = 1
      end
    end
    config.vm.define "webserver-two" do |app|
      app.vm.box = "bento/ubuntu-16.04"
      app.vm.network "private_network", ip: "192.168.33.13"
      app.vm.hostname = "webserver-two"
      app.vm.provider "virtualbox" do |v|
          v.memory = 512
          v.cpus = 1
        end
      end
    config.vm.define "debserver" do |app|
      app.vm.box = "bento/ubuntu-16.04"
      app.vm.network "private_network", ip: "192.168.33.14"
      app.vm.hostname = "debserver"
      app.vm.provider "virtualbox" do |v|
          v.memory = 512
          v.cpus = 1
        end
      end
  end
