# K8S Ansible playbook
This repository contain the automation files for deploying a K8S clustr on vCenter Environment.

## Ansible

Ansible files are available at the terraform directory. 

- [Supported Ansible Version](#supported-ansible-version)
- [Roles](#roles)
- [Ansible Roles Usage](#ansible-roles-usage)

### Supported Ansible Version

This ansible roles are tested using the following Ansible version:

```
$ ansible --version
ansible --version
ansible [core 2.12.1]
  config file = None
  configured module search path = ['/Users/melamin/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/local/Cellar/ansible/5.2.0/libexec/lib/python3.10/site-packages/ansible
  ansible collection location = /Users/melamin/.ansible/collections:/usr/share/ansible/collections
  executable location = /usr/local/bin/ansible
  python version = 3.10.1 (main, Dec  6 2021, 23:19:43) [Clang 12.0.0 (clang-1200.0.32.29)]
  jinja version = 3.0.3
  libyaml = True
```

### Roles

There is 1 roles that is part of this repository.

1. **k8s-role**


### Ansible Roles Usage

1. Pull the git repo:

```
$ git clone https://github.com/mohanadelamin/k8s-ansible-playbook.git

```

2. Change the variable on the following files to meet your requirements.
```
- hosts
- metallb/vars/main.yml
- kubernets/defaults/main.yml


3. Run the ansible play-book:

```
$ ansible-playbook k8s.yaml
```