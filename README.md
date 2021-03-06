docker-workshop
===============


To get started:

#### 1. Clone this repo:
```git clone https://github.com/bekkopen/docker-workshop.git```

#### 2. Install VirtualBox
Install VirtualBox from https://www.virtualbox.org/wiki/Downloads

#### 3. Install vagrant
Install vagrant from https://www.vagrantup.com/ and fetch our Docker-ready 
vagrant image by running 
```
cd docker-workshop
vagrant up
```

#### 4. Pull docker base image
Inside the vagrant box, pull the ubuntu base image for Docker:
```
vagrant ssh
cd /vagrant
docker run ubuntu echo "hello world"
```

#### 5. Check out the presentation 
http://bekkopen.github.io/docker-workshop

#### Troubleshooting

##### Installing Vagrant or VirtualBox
If you are having trouble installing VirtualBox, Vagrant or the Vagrant Image, you can follow the official installation instructions on https://docs.docker.com/ 

##### Problems running vagrant up on Windows
Make sure virtualization is turned on in you BIOS

##### Port collision
If you already have mongodb running on your local machine, there will be a port collision when trying to run `vagrant up`. See this note from Torgeir on how to solve this: https://github.com/bekkopen/docker-workshop/issues/1#event-162609858
