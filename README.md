This is the project repository for deploying Floyd and Bender, the production and development Gopherbot instances in use at LinuxJedi.org. Published on GitHub based on my belief that working examples are the best documentation.

## Updating Floyd
From the Cloud9 'parsley' workstation:
```
parsley:~/git/deploy-gopherbot (master) $ ansible-playbook deploy.yaml -e target=floyd -e gopherbot_force_update=true
```

## Contents

* cloudconfig.yaml - data file used with `ruby-awstools` for managing cloudformation templates and ec2 instances
* static-hosts - scriptlet that tells Ansible to use `ansible_hosts.yaml`, for Cloud9 native instances where dynamic inventory doesn't work

## External Requirements

* lnxjedi.gopherbot Ansible role, https://github.com/lnxjedi/ansible-role-gopherbot
* ../aws-linuxjedi repository for `ruby-awstools`, https://github.com/parsley42/linuxjedi
* ../linuxjedi-private repository for `ruby-awstools`; private repo