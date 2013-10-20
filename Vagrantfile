Vagrant.configure("2") do |config|
  config.vm.box = "precise32"
  config.vm.box_url = "http://files.vagrantup.com/precise32.box"
  config.vm.provision "chef_solo" do |chef|
    chef.json = {

    }
  end
  config.vm.provision "shell", inline: "apt-get update"
  config.vm.provision "shell", inline: "apt-get -y install git vim"
  config.vm.provision "shell", inline: "cp /vagrant/bashrc /home/vagrant/.bashrc"
  config.vm.provision "shell", inline: "cp /vagrant/vimrc /home/vagrant/.vimrc"
end
