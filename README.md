Ops-task

Repository contains a Vagrantfile to create a simple Ubuntu Xenial64 machine using Ansible provisioning with following features.

  - Static IP
  - Two users : malhar anad jacopo
  - Passwordless authentication using SSH
  - Apache web server configured with site sighup.dev
  - Disabled root user login via SSH

### Steps to launch machine
- Download and install Vagrant from https://www.vagrantup.com/downloads.html
- Follow steps below to start machine 

Clone repository:
```sh
$ git clone https://github.com/vbmade2000/ops-task.git
```
Go to directory
```sh
$ cd ops-task
```
Up the machine using vagrant command. Vagrant will automatically download required image and start it
```sh
$ vagrant up
```

Add folowing entry  to /etc/hosts file of your host machine 
```sh
192.168.0.2 www.sighup.dev 
192.168.0.2 sighup.dev 
```
Open www.sighup.dev in your browser and voila you have super simple working site.

For any query feel free to contact me at vbmade2000@gmail.com

