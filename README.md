ansible-packer
=========

Install packer and default templates

Role Variables
--------------

`packer_version` : version of packer to install 

`packer_url` : download url for packer zip. can be found at https://www.packer.io/downloads.html

`packer_install_dir` : location to install packer binaries

`packer_template_dir` : location to install default Omnia packer build templates


Example:
```
packer_version: '0.8.6'
packer_url: "https://releases.hashicorp.com/packer/{{packer_version}}/packer_{{packer_version}}_linux_amd64.zip"
packer_install_dir: '/usr/local/bin'
packer_template_dir: '/opt/packer'
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: reactiveops.packer, packer_version: '0.8.6' }
