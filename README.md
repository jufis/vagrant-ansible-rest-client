# Provision docker-rest-server with vagrant and ansible

In this example we use the docker-rest-client project as our target module to run using vagrant and ansible.

##Requirements

Please install the following packages to your local linux environment:

<pre>
yum install vagrant
yum install VirtualBox
yum install cowsay.noarch
<pre>

Every time ansible strikes a cow will tell you what's going on:

<pre> _________________________________________________ 
< TASK: xxxxx | install required  packages       >
 ------------------------------------------------- 
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
</pre>

##Install latest ansible

Latest Ansible uses a2x which you can find on if you install the following package:

<pre>
sudo yum install first this one : asciidoc-8.6.8-2.fc20.noarch
</pre>

Build altest ansible as follows:

<pre>
git clone git://github.com/ansible/ansible.git --recursive
cd ./ansible
make rpm
sudo rpm -Uvh ./rpmbuild/ansible-*.noarch.rpm
</pre>

##VirtualBox Operating System

Latest fedora rawhide 64-bit bleeding edge OS custom build as of MAY 2015 :)

##Box Location

https://github.com/jufis/vagrant-rawhide-box

##Vagrant version

>$ vagrant --version

<pre>
ansible 2.0.0
  configured module search path = None
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
