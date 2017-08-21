Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-6.9"

  config.vm.define "prd_web" do |prd_web|
    prd_web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2022
    prd_web.vm.network :private_network, ip: "192.168.101.11"
  end

  config.vm.define "prd_db" do |prd_db|
    prd_db.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2023
    prd_db.vm.network :private_network, ip: "192.168.101.12"
  end

  config.vm.define "test_web" do |test_web|
    test_web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2024
    test_web.vm.network :private_network, ip: "192.168.102.11"
  end

  config.vm.define "test_db" do |test_db|
    test_db.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2025
    test_db.vm.network :private_network, ip: "192.168.102.12"
  end

end
