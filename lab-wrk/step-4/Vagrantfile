Vagrant.configure("2") do |config|

    config.vm.box = "maier/alpine-3.4-x86_64"

    # for Alpine Linux...
    config.vm.synced_folder '.', '/vagrant', disabled: true

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
        ansible.sudo = true
        ansible.extra_vars = { alpine_python_fix_repo: true }
    end

end
