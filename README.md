
# cloud-to-edge

This is a meta repository to link all repositories required for the
_Cloud-to-Edge_ project.

## Overview

The current Git repositories in this project are as follows:

| Project       | Status        | Usage            |
| ------------- | ------------- | ---------------- |
| [Azure Edge](https://github.com/vmware/ansible-role-microsoft-role-azure-edge) | [![Build Status](https://travis-ci.org/vmware/ansible-role-microsoft-azure-edge.svg?branch=master)](https://travis-ci.org/vmware/ansible-role-microsoft-azure-edge) | Azure Edge automated install |
| [Azure IoT](https://github.com/vmware/ansible-role-microsoft-azure-iot) | [![Build Status](https://travis-ci.org/vmware/ansible-role-microsoft-azure-iot.svg?branch=master)](https://travis-ci.org/vmware/ansible-role-microsoft-azure-iot) | Azure IoT API automation |
| [Cloud-to-Edge VM](https://github.com/vmware/ansible-role-cloud-to-edge-vm) | [![Build Status](https://travis-ci.org/vmware/ansible-role-cloud-to-edge-vm.svg?branch=master)](https://travis-ci.org/vmware/ansible-role-cloud-to-edge-vm) | Create Cloud-to-Edge VMs |
| [Ansible Greengrass](https://github.com/vmware/ansible-aws-greengrass) | [![Build Status](https://travis-ci.org/vmware/ansible-aws-greengrass.svg?branch=master)](https://travis-ci.org/vmware/ansible-aws-greengrass) | AWS Greengrass automation |
| [Cloud-to-Edge Automation](https://github.com/vmware/cloud-to-edge-automation) | [![Build Status](https://travis-ci.org/vmware/cloud-to-edge-automation.svg?branch=master)](https://travis-ci.org/vmware/cloud-to-edge-automation) | Wrapper project for all automation |
| [VMware PKS Concourse Deploy](https://github.com/vmware/vmware-pks-deploy) | [![Build Status](https://travis-ci.org/vmware/vmware-pks-deploy.svg?branch=master)](https://travis-ci.org/vmware/vmware-pks-deploy) | VMware Concourse Builder, adapted for C2E deploy instead |
| [Cloud-to-Edge Concourse Deploy](https://github.com/vmware/cloud-to-edge-concourse-deploy) | [![Build Status](https://travis-ci.org/vmware/cloud-to-edge-concourse-deploy.svg?branch=master)](https://travis-ci.org/vmware/cloud-to-edge-concourse-deploy) | Cloud-to-Edge specific Concourse pipelines |

## Try it out

***Do not clone this repository.***
Instead, [install Google Repo](https://source.android.com/source/downloading#installing-repo) and use that to source all the component git repositories.

Here's a quick google repo install for the impatient.

```bash
# Validate python
python2.7 -c "print 'Python OK'" || echo 'Need python 2.7!'
python --version 2>&1 | grep -q "Python 2" || echo 'Warning: python 3 is default!'
mkdir ~/bin
PATH=~/bin:$PATH
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
# If you get a warning that about python 3, you might run this:
# After repo is installed:
sed -ri "1s:/usr/bin/env python:/usr/bin/python2.7:" ~/bin/repo
```

### Prerequisites

* Google Repo (and it's requirements)
* Git
* Access to one or more vCenters

### Build & Run

Once you've installed Git Repo, create and/or change into a directory where
you'd like to place all source relevant to this demo and execute -

`repo init -u https://github.com/vmware/cloud-to-edge`

...followed by...

`repo sync`

After the sync completes, navigate to the newly created
`c2e-deploy/bootstrap` directory and follow the instructions in that README.

## Documentation

## Releases & Major Branches

## Contributing

The cloud-to-edge project team welcomes contributions from the community. If you wish to contribute code and you have not
signed our contributor license agreement (CLA), our bot will update the issue when you open a Pull Request. For any
questions about the CLA process, please refer to our [FAQ](https://cla.vmware.com/faq). For more detailed information,
refer to [CONTRIBUTING.md](CONTRIBUTING.md).

## License

BSD-2
