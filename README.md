TrueSight Pulse Vagrant Docker
--------------------------------

Configures a virtual machine with a Docker daemon running at localhost:2375 for testing TrueSight Pulse Plugin for Docker.

## Prerequistes

- Vagrant 1.72. or later, download [here](https://www.vagrantup.com/downloads.html)
- Virtual Box 4.3.26 or later, download [here](https://www.virtualbox.org/wiki/Downloads)
- git 1.7 or later

## Installation

Prior to installation you need to obtain in your Boundary API Token.

1. Clone the GitHub Repository:

     ```bash
     $ git clone https://github.com/boundary/truesightpulse-vagrant-docker
     ```

2. Start the virtual machine using your TrueSight Pulse API Token:

    ```bash
     $ API_TOKEN=<TrueSight Pulse API Token> vagrant up <virtual machine name>
    ```
    NOTE: Run `vagrant status` to list the name of the virtual machines.

    Optionally provide the version of docker you want to install:

    ```bash
    $ API_TOKEN=<TrueSight Pulse API Token> DOCKER_VERSION=<docker version> vagrant up <virtual machine name>
    ```

3. Login to the virtual machine

    ```bash
    $ vagrant ssh <virtual machine name>
    ```
