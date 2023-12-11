
Vagrant.configure("2") do |config|
  config.vm.define "server1" do |server1|
    server1.vm.box = "ubuntu/focal64"
    server1.vm.network "public_network", ip: "192.168.1.213", bridge: "wlp9s0", auto_config: false
    server1.vm.synced_folder "site/", "/var/website"
    server1.vm.provision "shell", path: "script.sh"
        
     end

  config.vm.provider "virtualbox" do |server1|
    server1.memory = 2048
    server1.cpus = 2
    server1.name = "maquina-vitual-01.1"
    end

end
