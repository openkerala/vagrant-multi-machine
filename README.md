# Project Title

Setup multiple machines with vagrant and virtualbox. Also capable of assigning private IP addresses.

## Getting Started



### Prerequisities and Install

Trying this on ubuntu Xenial 16.04, Virtualbox (came with default repository) and Vagrant

```
sudo apt-get install virtualbox vde2 virtualbox-guest-additions-iso
sudo dpkg -i vagrant_1.8.4_x86_64.deb
vagrant box add ubuntu/xenial64
vagrant box add centos/7
```

### Fireup the instances
Command to fireup the instance from with the folder where Vagrantfile resides
```
vagrant up
```


