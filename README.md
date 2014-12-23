# kubernetes-on-coreos

Running Google kubernetes on CoreOS with Vagrant and VirtualBox.

## Quick Start

**Install [Vagrant](https://www.vagrantup.com/)**

**Install [VirtualBox](https://www.virtualbox.org/)**

```
$ git clone https://github.com/chengweiv5/kubernetes-on-coreos.git
$ cd kubernetes-on-coreos
```

### Start kubernetes master node

$ cd master
$ vagrant up

This will start kubernetes master node with IP:*172.17.8.141*, you may
change it in *master/Vagrantfile*.

### Start kubernetes minion nodes

$ cd minion
$ vagrant up

This will start *3* kubernetes minion nodes with IP:

- 172.17.8.146
- 172.17.8.147
- 172.17.8.148

You may change them in *minion/Vagrantfile*. See *minion/config.rb* if
you want to change how many minions or CoreOS channel or any more.
