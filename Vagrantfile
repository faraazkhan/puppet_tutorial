box      = 'precise32'
url      = 'http://files.vagrantup.com/precise32.box'
hostname = 'puppettutorialvagrant'
domain   = 'example.com'
ip       = '192.168.0.42'
ram      = '256'

Vagrant::Config.run do |config|
  config.vm.box = box
  config.vm.box_url = url
  config.vm.host_name = hostname + '.' + domain
  config.vm.network :hostonly, ip

  config.vm.customize [
    'modifyvm', :id,
    '--name', hostname,
    '--memory', ram
  ]

end
