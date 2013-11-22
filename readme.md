# Ansible Playbook for Modx Revolution

## Vagrant

Install [Vagrant](http://www.vagrantup.com/) and use ```vagrant up``` to create the server.

The setup playbook authorizes your local user for SSH login via ```allowed_hosts``` and assumes you have a public key created.

```ansible-playbook -c paramiko -i setup/hosts setup/setup.yml --ask-pass --sudo```

When prompted for password, use ```vagrant```

## Remote host

Modify the ```hosts``` file, or simply set up your ```/etc/ansible/hosts``` and disregard the ```-i``` in the playbook command.

```ansible-playbook -i hosts modx.yml```
