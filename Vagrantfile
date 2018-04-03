# Every Vagrant virtual environment requires a box to build off of.
# config.vm.box = "base"

Vagrant.configure(2) do |config|
    config.vm.define "mon" do |mon|
        mon.vm.hostname = 'monitoring'
        mon.vm.box      = 'gbarbieru/xenial'
        mon.vm.network "public_network" , ip: "192.168.100.115"
            config.vm.provider "mon" do |mon|
                mon.memory = "2048"
                mon.cpus = "2"
            end
    end

    config.vm.define :web do |web|
        web.vm.hostname = "web"
        web.vm.box      = 'gbarbieru/xenial'
        web.vm.network "public_network" , ip: "192.168.100.116"
            config.vm.provider "web" do |web|
                web.memory = "2048"
                web.cpus = "2"
            end
    end


    config.vm.define :mon2 do |mon2|
        mon2.vm.hostname = "mon2"
        mon2.vm.box      = 'gbarbieru/xenial'
        mon2.vm.network "public_network" , ip: "192.168.100.116"
            config.vm.provider "mon2" do |mon2|
                mon2.memory = "2048"
                mon2.cpus = "2"
            end
    end 
end
