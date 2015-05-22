# Provision docker-rest-server with vagrant and ansible

In this example we use the docker-rest-client project as our target module to run using vagrant and ansible.

##Requirements

Please install the following packages to your local linux environment:

<pre>
yum install vagrant
yum install ansible
yum install VirtualBox
yum install python-docker-py
<pre>

##VirtualBox Operating System

CentOS 7 64-bit

##Box Location

https://github.com/holms/vagrant-centos7-box/releases/download/7.1.1503.001/CentOS-7.1.1503-x86_64-netboot.box

##Vagrant version

>$ vagrant --version

<pre>
Vagrant 1.7.2
</pre>

##Ansible version

>$ ansible --version

<pre>
ansible 1.9.1
  configured module search path = None
</pre>


##Instructions

You need to edit the following to match your environment:

1. Vagrantfile
2. docker-rest-client.yml
3. roles/docker-rest-client/vars/main.yml
