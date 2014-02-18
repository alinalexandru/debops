# -*- mode: ruby -*-
# vi: set ft=ruby

# Vagrantfile for ginas project
# https://github.com/drybjed/ginas/

VAGRANTFILE_API_VERSION = '2'

DOMAIN = '.nat.example.com'
NETWORK = '192.168.50.'
NETMASK = '255.255.255.0'

# Source: https://github.com/drybjed/vagrant-debian-wheezy-64/tree/ginas
DEFAULT_BOX = 'debian-wheezy-amd64-netinst'
DEFAULT_BOX_URL = 'https://dl.dropboxusercontent.com/u/55426468/debian-wheezy-amd64-netinst.box'

# Fix permissions of vagrant's insecure SSH key
system('chmod 0600 contrib/vagrant/ssh/id_rsa_insecure')

# Load Vagrantfile from currently active Ansible inventory
begin
    load 'inventory-vagrant/Vagrantfile'
rescue LoadError
    # ignore
end


