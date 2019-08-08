### Humio test VM 1

Vagrant.configure("2") do |config|
  config.vm.box = "https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64-vagrant.box"
  # Use a private network so that we don't have to worry about forwarding ports
  config.vm.network "private_network", ip: "192.168.100.11"
  config.vm.define "humio-test1"
  config.vm.hostname = "humio-test1"
  config.vm.provider "virtualbox" do |v|
  config.disksize.size = "50GB"
    v.memory = 8192
    v.cpus = 4
    v.customize [ "guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 1000 ]
  end
  config.vm.provision :shell, path: "bootstrap.sh"
end

### Humio test VM 2

Vagrant.configure("2") do |config|
  config.vm.box = "https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64-vagrant.box"
  # Use a private network so that we don't have to worry about forwarding ports
  config.vm.network "private_network", ip: "192.168.100.12"
  config.vm.define "humio-test2"
  config.vm.hostname = "humio-test2"
  config.vm.provider "virtualbox" do |v|
  config.disksize.size = "50GB"
    v.memory = 8192
    v.cpus = 4
    v.customize [ "guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 1000 ]
  end
  config.vm.provision :shell, path: "bootstrap.sh"
end

### Humio test VM 3

Vagrant.configure("2") do |config|
  config.vm.box = "https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64-vagrant.box"
  # Use a private network so that we don't have to worry about forwarding ports
  config.vm.network "private_network", ip: "192.168.50.13"
  config.vm.define "humio-test3"
  config.vm.hostname = "humio-test3"
  config.vm.provider "virtualbox" do |v|
  config.disksize.size = "50GB"
    v.memory = 8192
    v.cpus = 4
    v.customize [ "guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 1000 ]
  end
  config.vm.provision :shell, path: "bootstrap.sh"
end
