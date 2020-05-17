Vagrant.configure("2") do |config|
  config.vm.box = "ysz/focal64"
  config.vm.box_version = "20200507.0.0"

  config.vm.provider "vmware_desktop" do |v|
    v.gui = true
    v.vmx["memsize"] = "4096"
  end

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get install -y libelf-dev cmake build-essential linux-headers-$(uname -r) pkg-config
  SHELL
end
