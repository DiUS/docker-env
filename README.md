Docker playground
=================

Setup
-----

* [Install VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Install Vagrant](http://docs.vagrantup.com/v2/installation/)
* [Install git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* Get the content of this git repository:
 * git clone https://github.com/DiUS/docker-env.git
 * OR [download a ZIP](https://github.com/DiUS/docker-env/archive/master.zip)
   and extract it
* In a shell run
    ```shell
    vagrant plugin install vagrant-vbguest
    ```
 * If this last step didn't work: don't worry... it's not the end of the world.

Running the virtual box
----

* open a shell
* change into the directory you downloaded the git repository into (or unziped)
* run `vagrant up`
 * It will download the box. This takes a while since the size is about 1.6 GB
 * If the process asks you for a password: *vagrant*
* Inside the box you should be able to login with username: vagrant and
  password: vagrant
* Open a shell *SCREEN_HERE*
* enter `docker run --rm -i -t ubuntu:14.04 /bin/bash`
* inside the docker container enter `ping google.com`