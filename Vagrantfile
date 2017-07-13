# Vagrantfile to create Ubuntu xenial64 

Vagrant.configure(2) do |config|

    config.vm.box = "ubuntu/xenial64"
    config.vm.network "private_network", ip: "192.168.0.2"
    config.vm.hostname = "mymachine"
    config.vm.synced_folder "shared/", "/home/ubuntu/shared"
    config.vm.network "forwarded_port", guest: 80, host: 80


    # Configuration for provider
    config.vm.provider "virtualbox" do |vbox|
    	vbox.gui = false
    	vbox.memory = 2048

    end

end
