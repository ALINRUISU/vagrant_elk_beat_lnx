Vagrant.configure("2") do |config|
  config.vm.define "elk01", primary: true do |elk01|
    elk01.vm.box = "centos/7"
    elk01.vm.hostname = 'elk01'

    elk01.vm.network :public_network, ip: "192.168.0.191"

    elk01.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      v.customize ["modifyvm", :id, "--memory", 2048]
      v.customize ["modifyvm", :id, "--name", "elk01"]
    end
    #config.vm.provision :shell, path: "bootstrap.sh"

  end

  config.vm.define "elk02" do |elk02|
    elk02.vm.box = "centos/7"
    elk02.vm.hostname = 'elk02'

    elk02.vm.network :public_network, ip: "192.168.0.192"

    elk02.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      v.customize ["modifyvm", :id, "--memory", 2048]
      v.customize ["modifyvm", :id, "--name", "elk02"]
    end
    #config.vm.provision :shell, path: "bootstrap.sh"

  end

  config.vm.define "elk03" do |elk03|
    elk03.vm.box = "centos/7"
    elk03.vm.hostname = 'elk03'

    elk03.vm.network :public_network, ip: "192.168.0.193"

    elk03.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      v.customize ["modifyvm", :id, "--memory", 2048]
      v.customize ["modifyvm", :id, "--name", "elk03"]
    end
    #config.vm.provision :shell, path: "bootstrap.sh"

  end

end