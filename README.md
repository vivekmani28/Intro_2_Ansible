# Intro_2_Ansible

## Ansible play book
The play book is attached in this repo.(file name: firstplaybook.yml). This is a very simple playbook demonstrating the use of ansible for configuration management. It demonstrates apt, git and shell modules.

## Steps for running the playbook

1. Initialize an instance of ubuntu/trusty64 using vagrant.
2. Have anisble installed in that server, the master server and connect to all the clients.
3. Initialize another instance of ubuntu/trusty64 using vagrant. This server will be like a client server.
4. Set up passwordless log-in for the client server in the master server by using the client's private key copied to the master.
5. Add the server details in the inventory file.
6. Initialize more client servers if required and perform step 4-5 once again.
7. Once done with setting up the clients, execute the anisible playbook using the below command

``
   ansible-playbook -i inventory -s firstplaybook.yml
``

