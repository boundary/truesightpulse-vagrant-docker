TrueSight Pulse Vagrant Docker
--------------------------------

Configures a virtual machine with a Docker daemon running at localhost:2375 for testing TrueSight Pulse Plugin for Docker.

## Prerequistes

- Vagrant 1.72. or later, download [here](https://www.vagrantup.com/downloads.html)
- Virtual Box 4.3.26 or later, download [here](https://www.virtualbox.org/wiki/Downloads)
- git 1.7 or later

## Installation

Prior to installation you need to obtain in your TrueSight Pulse API Token. The API Token is available by logging into your TrueSight Pulse account and navigating to _Settings_ -> _Account_.

1. Clone the GitHub Repository:

     ```bash
     $ git clone https://github.com/boundary/truesightpulse-vagrant-docker
     ```

2. Start the virtual machine using your TrueSight Pulse API Token and selecting the virtual machine name (Run `vagrant status` to list the name of the virtual machines):

    __Unix and Linux__

    ```bash
     $ API_TOKEN=<TrueSight Pulse API Token> vagrant up <virtual machine name>
    ```
    __Windows__

    ```bash
    C:\Users\demo> set API_TOKEN=<TrueSight Pulse API Token>
    C:\Users\demo> vagrant up <virtual machine name>
    ```

    Optionally provide the version of docker you want to install by setting the environment variable `DOCKER_VERSION`. If the environment variables is not set the Docker version defaults to 1.7.1

3. Login to the virtual machine

    ```bash
    $ vagrant ssh <virtual machine name>
    ```
