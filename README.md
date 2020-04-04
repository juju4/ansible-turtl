[![Build Status - Master](https://travis-ci.org/juju4/ansible-turtl.svg?branch=master)](https://travis-ci.org/juju4/ansible-turtl)
[![Build Status - Devel](https://travis-ci.org/juju4/ansible-turtl.svg?branch=devel)](https://travis-ci.org/juju4/ansible-turtl/branches)

# Turtl server install

This role installs Turtl Server from https://github.com/turtl/server

# Requirements & Dependencies

### Ansible
It was tested on the following versions:
 * 2.9

### Operating systems

Tested with molecule on Ubuntu 18.04

## Example Playbook

Just include this role in your list.
For example

```
- host: all
  roles:
    - juju4.turtl
```

## Continuous integration

This role has a travis config leveraging molecule for testing

Once you ensured all necessary roles are present, You can test with:
```
$ pip install molecule docker
$ molecule test
$ MOLECULE_DISTRO=ubuntu:18.04 molecule test --destroy=never
```

## Troubleshooting & Known issues

## License

BSD 2-clause
