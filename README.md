## Install vagrant 

Follow instructions in the following link to install https://www.vagrantup.com/downloads

## Find the appropriate box

Go to https://vagrantcloud.com/search to search the box containing the OS you 
want to have in your VM.

In the following example we choose ubuntu 20.10 which correspond to ubuntu/impsh64

## init Vagrant

```
vagrant init ubuntu/impish64
```

## Start VM

```
vagrant up
```

### vagrant provision

You can uncomment lines 66-69 in Vagrantfile to enable VM provision. 
You can add software install commands after line 68.

```
vagrant provision
```

### disable or enable GUI

GUI is disable by default. If you want to enable GUI, uncomment lines 52-58.

### to stop VM

To stop the VM use the following command: 

```
vagrant halt
```

### To connect to the VM

```
vagrant ssh
```

## Packaging the box

Vagrant include a simple way to package Virtualbox base boxes.

```
vagrant package --base my-virtual-machine

```

Where my-virtual-machine in the name of the virtual machine in Virtualbox to package as a base box.


