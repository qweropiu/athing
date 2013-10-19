Vagrant.configure("2") do |config|
  config.vm.box = "lucid32"
  config.vm.box_url = "http://files.vagrantup.com/lucid32.box"
  config.vm.provision "chef_solo" do |chef|
    chef.add_recipe "git"
    chef.add_recipe "vim"
    chef.add_recipe "build-essentials"
    chef.add_recipe "python::source"
    chef.json = {
      "python" => {
        "version" => "2.7.5"
      }
    }
  end
end
