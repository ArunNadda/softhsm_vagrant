# -*- mode: ruby -*-
# vi: set ft=ruby :


# Define Vault Primary HA server details
VAULT_HSM_IP_PREFIX = ENV['VAULT_HSM_IP_PREFIX'] || "10.10.42.10"
VAULT_HSM_IPS = ENV['VAULT_HSM_IPS'] || '"10.10.42.100", "10.10.42.101"'


Vagrant.configure("2") do |config|
  config.vm.box = "bento/debian-9"

  # set up the 2 node Vault Primary HA servers
  #(0).each do |i|
    config.vm.define "softhsm1" do |v1|
      v1.vm.hostname = "softhsm1"
      
      v1.vm.network "private_network", ip: VAULT_HSM_IP_PREFIX+"1"
      v1.vm.provision "shell", path: "setup_softhsm.sh"
    end
  #end
end
