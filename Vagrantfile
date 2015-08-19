Vagrant.configure("2") do |abc|
  abc.vm.box = "vagranttestbox"
  abc.vm.box_url = "http://192.168.1.3/demobox.box"
  abc.vm.provision :shell, :path => "setup.sh"
  abc.vm.network "forwarded_port", guest: 80, host: 6060
  abc.vm.network "forwarded_port", guest: 8080, host: 5050
  abc.vm.network "forwarded_port", guest: 2812, host: 2812
end
