Vagrant.configure("2") do |config|

  # Scriptbox configuration
  config.vm.define "scriptbox" do |scriptbox|
    scriptbox.vm.box = "alpine-linux/alpine-x86_64" # Alpine Linux
    scriptbox.vm.box_version = "3.12.0"
    scriptbox.vm.network "private_network", ip: "192.168.10.12"
    scriptbox.vm.hostname = "scriptbox"
    scriptbox.vm.provider "libvirt" do |vb|
      vb.memory = "512"
    end
  end

  # Web01 configuration
  config.vm.define "web01" do |web01|
    web01.vm.box = "generic/centos9s" # CentOS 9 Stream
    web01.vm.box_version = "4.3.12"
    web01.vm.network "private_network", ip: "192.168.10.13"
    web01.vm.hostname = "web01"
    web01.vm.provider "libvirt" do |vb|
      vb.memory = "512"
    end
  end

  # Web02 configuration
  config.vm.define "web02" do |web02|
    web02.vm.box = "generic/fedora38" # Fedora 38
    web02.vm.box_version = "4.3.12"
    web02.vm.network "private_network", ip: "192.168.10.14"
    web02.vm.hostname = "web02"
    web02.vm.provider "libvirt" do |vb|
      vb.memory = "512"
    end
  end

  # Web03 configuration
  config.vm.define "web03" do |web03|
    web03.vm.box = "generic/ubuntu1804" # Ubuntu 18.04
    web03.vm.box_version = "4.3.12"
    web03.vm.network "private_network", ip: "192.168.10.15"
    web03.vm.hostname = "web03"
    web03.vm.provider "libvirt" do |vb|
      vb.memory = "512"
    end
  end
end
