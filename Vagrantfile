# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "debian/bookworm64"

    config.vm.hostname = "dockerbox"

    config.vm.provision "shell", inline: <<-SHELL
        apt-get update && apt-get install -y docker.io docker-compose
        usermod -aG docker vagrant
    SHELL

    config.ssh.insert_key = false # This is usually recommended for base boxes
end
