# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-20.04"
  config.vm.hostname = "ServerTest"

   config.vm.provider "virtualbox" do |vb|
     vb.memory = "2048"
     vb.cpus = 2
   end

  config.vm.provision "shell", inline: <<-SHELL
    apt update
    apt install -y python3
  SHELL
end
