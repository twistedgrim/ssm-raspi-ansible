##### SSM-RASPI-Ansible

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
