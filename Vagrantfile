Vagrant.configure("2") do |config|
  config.vm.box = "fredrikhgrelland/hashistack"

  # Hashicorp consul ui
  config.vm.network "forwarded_port", guest: 8500, host: 8500, host_ip: "127.0.0.1"

  # Hashicorp nomad ui
  config.vm.network "forwarded_port", guest: 4646, host: 4646

  config.vm.provider "virtualbox" do |vb|
    vb.linked_clone = true
    vb.memory = 2048
  end
end