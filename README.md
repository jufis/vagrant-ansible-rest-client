# Provision docker-rest-client with vagrant and ansible

In this example we use the docker-rest-client project as our target module to run using vagrant and ansible.

Here I have used the following centos image:

https://github.com/holms/vagrant-centos7-box/releases/download/7.1.1503.001/CentOS-7.1.1503-x86_64-netboot.box

For local ansible I have used this version:

>$ ansible --version

<pre>
ansible 1.9.1
  configured module search path = None
</pre>

You need to edit the following to match your environment:

1. Vagrantfile
2. docker-rest-client.yml
3. roles/docker-rest-client/vars/main.yml
