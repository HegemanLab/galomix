# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/disco64"

  config.vm.network "forwarded_port", guest: 8080, host: 8181, host_ip: "127.0.0.1"

  config.vm.provider "virtualbox" do |v|
    v.memory = 2046
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "tests/playbook.yml"
    ansible.become = true
  end

  if Vagrant.has_plugin?("vagrant-cachier")
    config.cache.scope = :box
  end
end
