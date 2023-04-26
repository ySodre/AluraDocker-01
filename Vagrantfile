Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"


  config.vm.define "alura" do |alura|
    alura.vm.network "public_network", ip: "192.168.10.105"
    alura.vm.synced_folder "app-exemplo/", "/home/vagrant/app-exemplo"

  end

end