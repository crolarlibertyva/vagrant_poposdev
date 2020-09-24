Vagrant.configure("2") do |config|

   # Install Plugin to Resize Disk
  required_plugins = %w( vagrant-vbguest vagrant-disksize )
  
  config.vm.box = "tranchung/PopOS-2004-x64"
  config.disksize.size = "40GB"
  
  # VBoxManage for VM Customizations
  config.vm.provider :virtualbox do |vb|
    # Headless Mode
    vb.gui = true
    vb.name = "poposdev"
    # VBoxManage for VM Customizations
    vb.customize [
      "modifyvm", :id,
      "--memory", "4096"
    ]
    vb.customize ['modifyvm', :id, '--clipboard', 'bidirectional']
  end
end