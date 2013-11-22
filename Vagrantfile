Vagrant::Config.run do |config|
    config.vm.box = "precise64"
    config.vm.forward_port 80, 8080
    config.vm.network :hostonly, "33.33.33.10"
end
