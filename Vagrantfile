# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-16.04"

  config.ssh.insert_key = false
  config.vm.provider 'virtualbox' do |vb|
    vb.memory = 256
  end

  config.vm.define 'web1' do |web|
    web.vm.hostname = 'web1.ersolution.net'
    web.vm.network :private_network, ip: '192.168.33.111'
  end

  config.vm.define 'web2' do |web|
    web.vm.hostname = 'web2.ersolution.net'
    web.vm.network :private_network, ip: '192.168.33.112'
  end

  config.vm.define 'db1' do |db|
    db.vm.hostname = 'db1.ersolution.net'
    db.vm.network :private_network, ip: '192.168.33.121'
  end
end
