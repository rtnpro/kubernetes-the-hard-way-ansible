Vagrant.configure("2") do |config|
  config.vm.provider "libvirt" do |libvirt|
    libvirt.memory = 512
  end

  config.vm.define "controller0" do |controller0|
    controller0.vm.box = "centos/7"
    controller0.vm.hostname = "controller0"
    controller0.vm.network "private_network", ip: "192.168.2.2"
  end

  config.vm.define "controller1" do |controller1|
    controller1.vm.box = "centos/7"
    controller1.vm.network :private_network, ip: "192.168.2.3"
    controller1.vm.hostname = "controller1"
  end

  config.vm.define "controller2" do |controller2|
    controller2.vm.box = "centos/7"
    controller2.vm.network :private_network, ip: "192.168.2.4"
    controller2.vm.hostname = "controller2"
  end

  config.vm.define "worker0" do |worker0|
    worker0.vm.box = "centos/7"
    worker0.vm.network "private_network", ip: "192.168.2.5"
    worker0.vm.hostname = "worker0"
  end

  config.vm.define "worker1" do |worker1|
    worker1.vm.box = "centos/7"
    worker1.vm.network :private_network, ip: "192.168.2.6"
    worker1.vm.hostname = "worker1"
  end

  config.vm.define "worker2" do |worker2|
    worker2.vm.box = "centos/7"
    worker2.vm.network :private_network, ip: "192.168.2.7"
    worker2.vm.hostname = "worker2"
  end

  config.vm.define "load_balancer" do |load_balancer|
    load_balancer.vm.box = "centos/7"
    load_balancer.vm.network :private_network, ip: "192.168.2.8"
    load_balancer.vm.hostname = "load-balancer"
  end

  config.vm.define "client" do |client|
    client.vm.box = "centos/7"
    client.vm.network :private_network, ip: "192.168.2.9"
    client.vm.hostname = "client"
  end
end
