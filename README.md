check_gitlfs
===

[![Build Status](https://travis-ci.org/lsst-sqre/check-gitlfs.svg?branch=master)](https://travis-ci.org/lsst-sqre/check-gitlfs)

A nagios/icinga/sensu "plugin" for checking the function of a git lfs backed
repo.  IOW - check that a git lfs service is returning objects.

Usage
---

```bash
UNKNOWN- usage: check_gitlfs -u <git repo url> -I <path to object>
 -u [GIT REPO URL] -- URL to clone git repo from.
 -I [PATH LFS OBJECT] -- Path to lfs backed file within repo.
 -h -- Display this help message.

example:

  check_gitlfs -u https://github.com/lsst/afwdata.git -I CFHT/D2/sdss.dat
```
