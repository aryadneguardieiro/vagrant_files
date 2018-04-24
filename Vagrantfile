Vagrant.configure("2") do |config|
  config.vm.provision :shell, inline: "echo Starting Vagrant config"
  config.vm.box = "box-cutter/ubuntu1604-desktop"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
  end

  config.vm.define :kubemaster do |kubemaster|
    kubemaster.vm.network "public_network", bridge: "en1: Wi-Fi (AirPort)", ip: "192.168.0.51"

  end
end