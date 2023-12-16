Vagrant.configure("2") do |config|

  config.vm.box = "centos/7"

  config.vm.provision "shell", path: "provision.sh"

  config.vm.network "forwarded_port", guest: 80, host: 8888, host_ip: "127.0.0.1"

  config.vm.synced_folder "./content/", "/home/vagrant/shared/", type: "rsync"
end
