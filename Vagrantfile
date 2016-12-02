Vagrant.configure(2) do |config|
  config.vm.box = "centos/7"
  config.vm.provider "virtualbox" do |v|
    v.memory = 8 * 1024
    v.cpus = 2
  end

  config.ssh.insert_key = false

  config.vm.provision "ansible" do |ansible|
    ansible.verbose = ''
    ansible.playbook = 'playbook.yml'
  end
end
