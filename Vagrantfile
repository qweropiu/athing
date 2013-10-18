Vagrant.configure("2") do |config|
  config.vm.box = "lucid32"
  config.vm.box_url = "http://files.vagrantup.com/lucid32.box"
  config.vm.provision "chef_solo" do |chef|
    chef.add recipe "git"
    chef.add recipe "vim"
  end
end
