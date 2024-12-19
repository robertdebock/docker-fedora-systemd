Docker Fedora Systemd
=====================

This Dockerfile can build containers capable to use systemd.

[![fedora build status](https://img.shields.io/docker/cloud/build/robertdebock/fedora.svg)](https://hub.docker.com/repository/docker/robertdebock/fedora)

Branches
--------

This repository has multiple branches that relate to Fedora versions.

|Branch |Fedora Version|Docker image tag|
|-------|--------------|----------------|
|40     |40            |40              |
|master |latest (41)   |latest          |
|rawhide|rawhide (42)  |rawhide         |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```shell
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  robertdebock/fedora:rawhide
```
