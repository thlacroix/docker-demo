Vagrant.configure("2") do |config|
  config.vm.box = "phusion/ubuntu-12.04-amd64"
  config.vm.provision "docker",
    images: ["ubuntu:latest", "node:latest", "dockerfile/mongodb"]

  config.vm.network "private_network", ip: "192.168.59.103"

  config.vm.network "forwarded_port", guest: 2375, host: 2375
end
