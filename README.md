
# cloud-to-edge

This is a meta repository to link all repositories required for the
_Cloud-to-Edge_ project.

## Overview

The current Git repositories in this project are as follows:

| Project       | Status        | Usage            |
| ------------- | ------------- | ---------------- |
| [Azure Edge](https://gitlab.com/vmworld2018/ansible-role-azure-edge) | [![Build Status](https://gitlab.com/vmworld2018/ansible-role-azure-edge/badges/master/pipeline.svg)](https://gitlab.com/vmworld2018/ansible-role-azure-edge/commits/master) | Azure Edge automated install |
| [Azure IoT](https://gitlab.com/vmworld2018/ansible-role-azure-iot) | [![Build Status](https://gitlab.com/vmworld2018/ansible-role-azure-iot/badges/master/pipeline.svg)](https://gitlab.com/vmworld2018/ansible-role-azure-iot/commits/master) | Azure IoT API automation |
| [Skyway Edge VM](https://gitlab.com/vmworld2018/ansible-role-skyway-edge-vm) | [![Build Status](https://gitlab.com/vmworld2018/ansible-role-skyway-edge-vm/badges/master/pipeline.svg)](https://gitlab.com/vmworld2018/ansible-role-skyway-edge-vm/commits/master) | Create Skyway Edge VMs |
| [Ansible Greengrass](https://github.com/vmware/ansible-aws-greengrass) | [![Build Status](https://travis-ci.org/vmware/ansible-aws-greengrass.svg?branch=master)](https://travis-ci.org/vmware/ansible-aws-greengrass) | AWS Greengrass automation |
| [Skyway Automation](https://gitlab.com/vmworld2018/skyway-automation) | [![Build Status](https://gitlab.com/vmworld2018/skyway-automation/badges/master/pipeline.svg)](https://gitlab.com/vmworld2018/skyway-automation/commits/master) | Wrapper project for all automation |
| [VMware Concourse Deploy](https://gitlab.com/vmworld2018/vmware-concourse-deploy) | [![Build Status](https://gitlab.com/vmworld2018/vmware-concourse-deploy/badges/master/pipeline.svg)](https://gitlab.com/vmworld2018/vmware-concourse-deploy/commits/master) | VMware Concourse Builder |
| [Skyway Concourse Deploy](https://gitlab.com/vmworld2018/skyway-concourse-deploy) | [![Build Status](https://gitlab.com/vmworld2018/skyway-concourse-deploy/badges/master/pipeline.svg)](https://gitlab.com/vmworld2018/skyway-concourse-deploy/commits/master) | Skyway specific Concourse pipelines |

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
`skyway-deploy/bootstrap` directory and follow the instructions in that README.

## Documentation

## Releases & Major Branches

## Contributing

The cloud-to-edge project team welcomes contributions from the community. If you wish to contribute code and you have not
signed our contributor license agreement (CLA), our bot will update the issue when you open a Pull Request. For any
questions about the CLA process, please refer to our [FAQ](https://cla.vmware.com/faq). For more detailed information,
refer to [CONTRIBUTING.md](CONTRIBUTING.md).

## License

BSD-2
