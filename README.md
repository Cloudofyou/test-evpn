## test-evpn

### Summary:

This is an Ansible demo which configures four Cumulus VX switches in a 3 site, 2 switch-per-site, 1 router-per-site configuration with BGP using J2 / Jinja2 templates

### Network Diagram:

![Network Diagram](https://github.com/cloudofyou/test-evpn/blob/master/VHP-EVPN-Test.png)

### Initializing the Linux / libvirt demo environment:

First, make sure that the following is currently running on your machine:

1. This demo was tested on a Ubuntu 18.04 NUC w/ 4 cores and 32Gb of RAM

2. Following the instuctions at the following link:

https://docs.cumulusnetworks.com/cumulus-vx/Development-Environments/Vagrant-and-Libvirt-with-KVM-or-QEMU/

3. Download the latest Vagrant, 2.2.5, from the following location:

    https://www.vagrantup.com/

4 Copy the Git repo to your local machine:

    ```git clone https://github.com/cloudofyou/test-evpn```

5. Change directories to the following

    ```test-evpn```

6. Run the following:

    ```./start-vagrant-libvirt-poc.sh```

### Running the Ansible Playbook

1. SSH into the oob-mgmt-server:

    ```cd vx-libvirt-simulation```   
    ```vagrant ssh oob-mgmt-server```

2. Copy the Git repo unto the oob-mgmt-server:

    ```git clone https://github.com/cloudofyou/test-evpn```

3. Change directories to the following

    ```test-evpn/automation```

4. Run the following:

    ```./provision.sh```

