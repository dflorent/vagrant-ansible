Vagrant Ansible
===============

Vagrant development environment provisionned with Ansible.

## Requirements

- VirtualBox
- Vagrant
- Ansible

## Contents

- Git
- ZSH with Oh-my-zsh
- Tmux
- Ruby
- Sass
- Mailcatcher
- MySQL
- Apache2
- PHP
- Composer
- phpMyAdmin (optional)
- Node.js

## Usage

```
vagrant up
vagrant ssh
cd /vagrant
```

### Vagrantfile

```
# change these values
config.vm.network "private_network", ip: "192.168.33.xx"
config.vm.hostname = 'example.dev'
```

### MySQL

- MySQL user: root
- MySQL password: root

### Mailcatcher

```
# http://example.dev:1080

mailcatcher --foreground --http-ip=0.0.0.0
```

### Git

```
# ansible/group_vars/all.yml

# git
git_email: john@doe.com
git_name: Jonh Doe
```
