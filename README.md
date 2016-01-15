# ansible-vagrant

## About

vagrantのセットアップ用のansible-playbook

## Installation

- リポジトリとvagrantのセット

```sh
$ mkdir test
$ cd test
$ git clone https://github.com/gembaf/ansible-vagrant.git
$ vagrant init
```

- Vagrantfileの上書き

```sh
$ cp ansible-vagrant/Vagrantfile.sample Vagrantfile
```

- vagrantの起動

```sh
$ vagrant up --provider virtualbox
```

## Requirements

- vagrant
- VirtualBox
- ansible
