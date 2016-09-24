Vagrant.configure("2") do |config|

  config.vm.define "ubuntu_host1" do |ubuntu_host1|
    ubuntu_host1.vm.box = "ubuntu/xenial64"
    ubuntu_host1.vm.hostname = 'ubuntu-host1'
    ubuntu_host1.vm.box_url = "ubuntu/xenial64"

    ubuntu_host1.vm.network :private_network, ip: "192.168.56.101"

    ubuntu_host1.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      v.customize ["modifyvm", :id, "--memory", 512]
      v.customize ["modifyvm", :id, "--name", "ubuntu-host1"]
    end
  end

  config.vm.define "centos_host1" do |centos_host1|
    centos_host1.vm.box = "centos/7"
    centos_host1.vm.hostname = 'centos-host1'
    centos_host1.vm.box_url = "centos/7"

    centos_host1.vm.network :private_network, ip: "192.168.56.102"

    centos_host1.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      v.customize ["modifyvm", :id, "--memory", 512]
      v.customize ["modifyvm", :id, "--name", "centos-host1"]
    end
  end
end
