# vagrant-dockerbox

![icon](icon-128.png)

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dmotte/vagrant-dockerbox/release?logo=github&style=flat-square)](https://github.com/dmotte/vagrant-dockerbox/actions)
[![Vagrant Cloud](https://img.shields.io/badge/vagrant-dmotte/dockerbox-blue?logo=vagrant&style=flat-square)](https://app.vagrantup.com/dmotte/boxes/dockerbox)

:package: **Debian Vagrant box** with **Docker** (and **docker-compose**).

This project uses [geerlingguy/ansible-role-docker](https://github.com/geerlingguy/ansible-role-docker) to install _Docker_ and _docker-compose_ inside the VM.

> :package: This box is also on **Vagrant Cloud** as [`dmotte/dockerbox`](https://app.vagrantup.com/dmotte/boxes/dockerbox).

> :calendar: The build and release process of this Vagrant box is **triggered automatically every month** (thanks, [GitHub Actions](https://github.com/features/actions)! :smile:) to ensure that you get it with all the latest updated packages. See the [workflow file](.github/workflows/release.yml) for further information.

## Usage

Please refer to the :file_folder: `test` folder to see an example of how I use this box.
