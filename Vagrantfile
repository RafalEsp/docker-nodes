Vagrant.configure(2) do |config|
    (1..3).each do |i|
      config.vm.define "node#{i}" do |node|
        node.vm.box = "debian/stretch64"
        node.vm.network "private_network", ip: "10.0.0.10#{i}"
      end
    end
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
    config.vm.provision :ansible do |ansible|
        ansible.inventory_path = "provision/inventory/local/hosts"
        ansible.playbook = "provision/provision.yml"
    end
end