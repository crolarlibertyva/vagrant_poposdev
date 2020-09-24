Vagrant.configure("2") do |config|
 
  config.vm.box = "tranchung/PopOS-2004-x64"
  
  # VBoxManage for VM Customizations
  config.vm.provider :virtualbox do |vb|
    # Headless Mode
    vb.gui = true
    vb.name = "pdev"
    # VBoxManage for VM Customizations
    vb.customize [
      "modifyvm", :id,
      "--memory", "4096"
    ]
    vb.customize ['modifyvm', :id, '--clipboard', 'bidirectional']
  end
end
