Vagrant.configure("2") do |config|
  # Configuração da máquina virtual
  config.vm.box = "centos/7"
  config.vm.hostname = "sonarqube"
  config.vm.network "forwarded_port", guest: 9000, host: 9000, hostip: "127.0.0.1"
  config.vm.provision 'shell', path: "provision.sh"
  # Configuração de recursos da máquina virtual
  config.vm.provider "virtualbox" do |v|
    v.memory = "1024" # Tamanho da memória RAM em MB
  end
end