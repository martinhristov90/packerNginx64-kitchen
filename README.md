# How to create a vagrant base box

# Purpose

This repository's sole purpose is to demonstrate how to built a Vagrant box with virtual box provider using Packer which provides Nginx webserver.

# Technologies in use :

- Packer
- Vagrant
- VirtualBox
- Nginx

# How to install the needed technologies :

- [How to install Packer](https://www.packer.io/intro/getting-started/install.html)
- [How to install Vagrant](https://www.vagrantup.com/docs/installation/)
- [How to install VirtualBox](https://www.virtualbox.org/manual/ch02.html)


# How to use

- Clone this git repository using `git clone https://github.com/martinhristov90/packerNginx64.git `
- Switch into the directory of the project using : `cd packerNginx64`
- Let Packer build the Vagrant box for you using : `packer build templete.json`
- You should now have Vagrant box which upon booting starts Nginx web server.
- Use command `vagrant box add ubuntu-1604-vbox.box --name DESIRED_NAME` to add the box to Vagrant.
- List available boxes with `vagrant box list`, the imported box should be listed.
- In order to boot the box with Vagrant, Vagrantfile needs to be generated. Use `vagrant init -m`, to generate simple Vagrantfile
- Type `vagrant up`.

### NB : Make sure you execute the abovementioned commands in `packerNginx64` directory.


