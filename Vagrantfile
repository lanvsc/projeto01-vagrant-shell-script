Vagrant.configure("2") do |config|

  #Configurando VM
  config.vm.define:proj01 do |proj01_config|
    proj01_config.vm.box = "bento/ubuntu-22.04"
    proj01_config.vm.network "public_network"
      proj01_config.vm.provider "virtualbox" do |v|
      v.gui = true
      v.memory = "1024"
      v.cpus = "1"
    end
    proj01_config.vm.provision "shell", path: "provision.sh"  
  end
 end