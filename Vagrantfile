# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  config.vm.define "hashi" do |hashi|
    hashi.vm.box = "mrlesmithjr/trusty64"
    hashi.vm.hostname = "hashi"

    hashi.vm.network :private_network, ip: "192.168.202.201"

    hashi.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end
  config.vm.provision :shell, path: "provision.sh", keep_color: "true"
end
