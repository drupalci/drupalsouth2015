Vagrant.configure("2") do |config|
  config.vm.box      = 'hashicorp/precise64'
  config.vm.hostname = 'ds2015.dev'
  
  config.vm.network :private_network, :ip => "192.168.90.10"

  config.vm.synced_folder ".", "/var/www"
  
  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--cpus",   1 ]
    vb.customize ["modifyvm", :id, "--memory", 512 ]
  end

  config.vm.provision :shell, :path => "scripts/provision.sh"
end
