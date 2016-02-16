# Vagrant
A vagrant box for providing a sandboxed development environment for everything.

# Use

Install [Vagrant](https://www.vagrantup.com/), [Ansible](http://www.ansible.com/), and [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

Clone the `vagrant` repository into the top level folder of your projects (I have a nine-worlds folder that I use, so the subfolders include `vagrant` and `calendar` are in mine right now, for example).

In terminal, `cd` into the vagrant folder and run `vagrant up`.

Add `nineworlds.vb` to your HOSTS file with `192.168.10.50`.

You should now be able to go to `nineworlds.vb/[folder]` to view any of your projects.

# The Provisioning

It comes with Ansible provisioning, which sets up the base machine. Right now, it sets up a basic Nginx web server and Postgres database. If you add anything to the virtual machine, let me know and I can add it to the provisioner, or you can brave learning how to add to it (it's pretty easy, but there is a learning curve).
