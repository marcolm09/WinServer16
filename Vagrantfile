Vagrant.configure("2") do |config|

  config.vm.define "server" do |server|
    server.vm.box = "mwrock/Windows2016"
    server.vm.communicator = "winrm"
    server.vm.hostname = "server"
    server.vm.network "private_network", ip: "192.168.50.2"
  end

  config.vm.define "win10" do |win10|
    win10.vm.box = "opentable/win-10"
    win10.vm.communicator = "winrm"
    win10.vm.hostname = "win10"
    win10.vm.network "private_network", ip: "192.168.50.3"
  end

end
