## Ansible playbook to install Docker and Docker Compose on Ubuntu 12.04 - 16.04

Ansible version >= 1.9 required

### Ubuntu 12.04 - 15.10
Open `inventory` file and change `localhost` with your server's ip address.
Launch installation process with command:
`ansible-playbook playbook.yml -i inventory`

### Ubuntu 16.04
Open `inventory16.04` file and change `localhost` with your server's ip address.
Launch installation process with command:
`ansible-playbook playbook.yml -i inventory16.04`
