# Docker Playgroung
This solution is based on VirtualBox, Vagrant and Ansible. If You're working on Windows machine, this won't work.
Ansible is not supporting Windows as control machines (http://docs.ansible.com/ansible/latest/intro_installation.html#control-machine-requirements).

## Quick Start
1. clone repository:
    ```
    git clone https://github.com/RafalEsp/docker-nodes.git
    ```
2. If You don't have Vagrant installed yet, do it now.  You can find instructions here: https://www.vagrantup.com/downloads.html
3. If You don't have Ansible installed yet, do it now. Instructions here: http://docs.ansible.com/ansible/latest/intro_installation.html
4. Now You're ready! In terminal after `cd docker-nodes`, type `vagrant up` and enjoy the view of creation of Virtual Machines.
5. If everything goes well, after typing `vagrant status`, you should see 3, provisioned with docker engine, ready to use virtual machines. 

Feel free to suggest changes and improvements.