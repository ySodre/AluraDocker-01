Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"


  config.vm.define "alura" do |alura|
    alura.vm.network "public_network"
    alura.vm.synced_folder "app-exemplo/", "/home/vagrant/app-exemplo"
    alura.vm.provision "shell", path: "script.sh"

  end

end