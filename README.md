This is the project repository for deploying Floyd and Bender, the production and development Gopherbot instances in use at LinuxJedi.org. Published on GitHub based on my belief that working examples are the best documentation.

## Contents

* cloudconfig.yaml - data file used with `ruby-awstools` for managing cloudformation templates and ec2 instances

## External Requirements

* lnxjedi.gopherbot Ansible role, https://github.com/lnxjedi/ansible-role-gopherbot
* ../aws-linuxjedi repository for `ruby-awstools`, https://github.com/parsley42/linuxjedi
* ../linuxjedi-private repository for `ruby-awstools`; private repo