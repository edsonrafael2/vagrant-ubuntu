
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/focal64"

  config.vm.network "public_network", ip: "192.168.1.213", bridge: "enp058"

  config.vm.synced_folder "site/", "/var/website"

  config.vm.provider "virtualbox" do |vm|
    vm.name = "maquina-vitual-01.1"
    
 end

  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.cpus = 1
 end



end
