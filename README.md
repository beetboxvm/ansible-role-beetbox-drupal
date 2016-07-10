# Ansible Role: Beetbox Drupal

[![CircleCI](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-drupal.svg?style=svg)](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-drupal)

An Ansible role that creates a Drupal project on beetbox.

## Requirements

This role is specifically developed as an extension to beetbox -- https://github.com/drupalmel/beetbox

## Role Variables

Available variables are listed below, along with default values:

    drupal_install_profile: standard

The drupal install profile.

    drupal_enable_modules: []

List of modules to enable.

    drupal_account_name: admin

Admin username.

    drupal_account_pass: admin

Admin user password.

    drupal_install_site: no

Install Drupal.

    drupal_create_makefile: no

Create a default make file.

    drupal_build_makefile: no

Build a make file.

    drupal_makefile_path: "~/beetbox.make.yml"

The make file to build.

    drupal_make_core_branch: "8.2.x"

Default core branch.

    drupal_distro: no

Build Drupal distro.

    drupal_distro_makefile: /vagrant/drupal-org.make.yml

Distro make file.

    drupal_build_composer: no

Build Drupal composer project.

    drupal_composer_version: "8.x-dev"

Composer project version.

    drupal_composer_dependencies: []

Drupal composer dependencies.


# beetbox

https://github.com/beetboxvm/beetbox

## Requirements

* [Vagrant](https://www.vagrantup.com/) >= 1.8
* [Virtualbox](https://www.virtualbox.org/)
* [Vagrant Hostsupdater](https://github.com/cogitatio/vagrant-hostsupdater)
* [Vagrant Auto-network](https://github.com/oscar-stack/vagrant-auto_network)

## Quickstart

  1. Open terminal (or [git bash](https://msysgit.github.io/) for windows users) and run the following commands --

  ```
  git clone https://github.com/beetboxvm/ansible-role-beetbox-drupal.git drupal && cd $_
  vagrant up
  ```

  2. Go to http://drupal.local/

  ```
  username: admin
  password: admin
  ```

## License

MIT
