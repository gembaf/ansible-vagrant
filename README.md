# ansible-vagrant

## About

vagrantのセットアップ用のansible-playbook

## Installation

- リポジトリとvagrantのセット

```sh
$ mkdir test
$ cd test
$ git clone https://github.com/gembaf/ansible-vagrant.git
$ vagrant init ubuntu/trusty64
```

- Vagrantfileへの追記

```ruby
Vagrant.configure(2) do |config|

  ……

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible-vagrant/main.yml"
  end
end
```

- vagrantの起動

```sh
$ vagrant up --provider virtualbox
```

## Requirements

- vagrant
- VirtualBox
- ansible
