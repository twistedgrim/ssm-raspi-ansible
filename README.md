# SSM-RASPI-Ansible
[![Ansible Role](https://img.shields.io/ansible/role/21883.svg)](https://galaxy.ansible.com/twistedgrim/ssm-raspi-ansible/)
[![Ansible Role](https://img.shields.io/ansible/role/d/21883.svg)](https://galaxy.ansible.com/twistedgrim/ssm-raspi-ansible/)

This playbook is built to install the SSM agent on a raspberry pi.
This has been tested and works against Pi 3 / Pi 2 / Pi Zero.

The tasks are setup to replicate the [setup guide](http://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-install-ssm-agent.html#agent-install-raspbianjessie) from Amazon.

### Requirements
- Managed-Instance Activation Process on [Amazon](http://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-managedinstances.html)


### Role Variables
- download_url
  : Used as the download location for the ssm agent
- region
  : Used as region when registering the Managed-Instance
- code
  : Managed-Instance activation code
- id
  : Managed-Instance activation id

### Example Playbook

Included is example of how to use the installation as a role. The required variables are represented.

```
- hosts: all
    roles:
       - { role: ssm-raspi-ansible, code: aYkdHGO75iZjEIrJ5nxI, id: 0e93f33e-3cc1-4a82-b9e2-g83d43ca7831 }
```

### License

MIT
