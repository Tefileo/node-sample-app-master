Vagrant.configure("2") do |config|



  config.vm.box = "ubuntu/bionic64"
  config.vm.synced_folder "./files", "/home/vagrant/files"
  config.vm.provider "virtualbox" do |v|
     v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
     v.customize ["modifyvm", :id, "--natdnsproxy1", "on"]
   end
end
