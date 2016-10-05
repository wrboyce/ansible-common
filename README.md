wrboyce.common
==============

[![Build Status](https://travis-ci.org/wrboyce/ansible-common.svg)](https://travis-ci.org/wrboyce/ansible-common)

I doubt this play will be useful to anyone beyond perhaps as a teaching aide.
At the very least, you'd want to fork it.

Requirements
------------

* [Homebrew](http://brew.sh) (macOS)

Role Variables
--------------

Exposes variables to install packages from various sources:

| variable          | source        |
|-------------------|---------------|
| apt_requirements  | apt           |
| brew_requirements | homebrew      |
| pip2_requirements | python2 / pip |
| pip3_requirements | python3 / pip |
| cask_requirements | homebrew-cask |
| mas_requirements  | mac app store |

Example Playbook
----------------

    - hosts: all
      roles:
         - wrboyce.common

License
-------

Apache 2.0