
# Docker Image with oraclelinux7 base image 

This repo was created in order to test ansible roles with molecule.

## Build it locally

  docker build -t oraclelinux7img .
  docker run --rm --privileged  -ti -e container=docker  -v /sys/fs/cgroup:/sys/fs/cgroup  oraclelinux7img /usr/sbin/init
  #docker run --name oraclelinux7con -d -P oraclelinux7img
  #docker exec -it oraclelinux7con bash

## Use it from dockerhub

    https://hub.docker.com/repository/docker/lotusnoir/ansible_molecule_test_images:oraclelinux7
