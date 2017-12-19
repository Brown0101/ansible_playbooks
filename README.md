# Ansible Playbooks
-------------------

These are example playbooks for automation of Linux and Windows servers in an environment.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Linux:
* epel-release - manditory
* python-pip - manditory
* markupsafe
* xmltodict
* pywinrm - manditory
* ansible - manditory
* awscli
* boto and boto3
* vim - nice to have
* tree - nice to have

Windows
* configure to use winrm
```

### Installing

A step by step series of examples that tell you have to get a development env running

```
Linux:
* yum install epel-release -y
* yum install python-pip -y
* pip install markupsafe
* pip install xmltodict
* pip install pywinrm
* pip install ansible
* pip install awscli
* pip install boto
* pip install boto
```

Next

```
Windows
- Elevate PowerShell Prompt
* Configure network
** netsh advfirewall set allprofiles state off
* PowerShell should at least be 3.0 or higher
** $PSVersionTable
** powershell
** Enable-PSRemoting
* Demo is using basic login. Verify Basic is set to true.
# NOTE: Basic is not secure and you should use SSL certs for production.
** winrm get winrm/config
** Set-Item -Path "WSMan:\localhost\Service\Auth\Basic" -value True
** Set-Item -Path "WSMan:\localhost\Service\AllowUnencrypted" -value True
```

Reference:
Adrian (2016), My first steps with Ansible, https://wyssmann.com/my-first-steps-with-ansible/


## Built With

* [Ansible](https://www.ansible.com) - AUTOMATION FOR EVERYONE
* [Modules](http://docs.ansible.com/ansible/latest/list_of_all_modules.html) - All Modules
* [Python](https://www.python.org) - Python is a scripting language that Ansible is built on.
* [Pip](https://pip.pypa.io/en/stable/) - Used to install python packages.

## Authors

* **Dwayne Brown** - *Initial Work* - (https://github.com/Brown0101)

## Acknowledgments

* Adrian for his WinRM examples

