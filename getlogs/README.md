# Ansible Automation | gp.getlogs

## Environment Preparation / Git Clone
Before cloning this project, please prepare your environment as described below.
This procedure is mandatory to execute "ansible-test" command.

Create "ansible_collections" folder in your workspace with the following command 

```
$ mkdir -p ~/ansible_collections/sample
```

Clone the repository in the created folder

```
$ git clone https://github.com/gpillon/ansible-test
```

## Requirements

|Component |Version |
|--|--|
| python | PYTHON_VERSION |
| ansible | >= ANSIBLE_VERSION |
| molecule | >= MOLECULE_VERSION |

Further details are reported into "requirements.txt" file

## Collection Test

For testing purpose, see "roles" molecule tests

## Collection Build

    [user@localhost]# ansible-galaxy collection build

This command will produce a tar.gz file. To install an Ansible Collection, please refer to Ansible Galaxy documentation

# Changelog

|Version |Feature |
|--|--|
| 1.0.0 | First version |


# Dependencies

- TODO


# Sample Playbook (imported as role)

    TODO : write here your sample playbook