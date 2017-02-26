docker-jenkins-service [![Build Status](https://travis-ci.org/bronzdoc/jenkins-docker-service.svg?branch=master)](https://travis-ci.org/bronzdoc/jenkins-docker-service)
=========

Jenkins in docker as a systemd service

Requirements
------------

Docker

Role Variables
--------------

| Variable | Meaning        | Default   |
|:-------|:-----------------|:-----------
| jenkins_home     | Path to your jenkins home | $HOME/jenkins_home
| jenkins_port     | Port mapping of you jenkins server container | 8080:8080


Example Playbook
----------------

    - hosts: hosts
      roles:
         - { role: docker-jenkins-service }

```
$ ansible-playbook --ask-sudo playbok.yml
```

Note: you need to `--ask-sudo` to configure the systemd unit properly

License
-------

MIT

Author Information
------------------

bronzdoc

