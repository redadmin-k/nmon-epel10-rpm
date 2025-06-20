nmon-epel10-rpm
===============

This repository contains RPM packaging files and build logs for "nmon"
(version 16p), targeting EPEL 10 and AlmaLinux 10 systems.

Package Overview
----------------
- Name       : nmon
- Version    : 16p
- Release    : 5.el10
- Architecture: x86_64
- Upstream   : https://nmon.sourceforge.net/pmwiki.php

Included Files
--------------
- nmon.spec                  : RPM spec file
- lmon16p.c                  : Upstream source
- nmon.1                     : Manual page
- nmon-16p-5.el10.src.rpm    : Source RPM
- nmon-16p-5.el10.x86_64.rpm : Binary RPM
- nmon-debuginfo-*.rpm       : Debug info package
- nmon-debugsource-*.rpm     : Debug source package
- build.log                  : Build log from mock
- root.log                   : Root log from mock
- state.log                  : Build state
- installed_pkgs.log         : Installed packages in chroot
- hw_info.log                : Hardware information from mock
- Documentation.txt          : Supplemental information

Build Instructions
------------------
This package was built using mock for EPEL 10:

  mock -r epel-10-x86_64 --rebuild nmon-16p-5.el10.src.rpm

Make sure you have mock installed and properly configured.

Installation
------------
To install the built package:

  sudo dnf install ./nmon-16p-5.el10.x86_64.rpm

To run nmon:

  nmon

License
-------
nmon is distributed under a restrictive license (non-GPL).
Please verify licensing terms at the official site:

  https://nmon.sourceforge.net/pmwiki.php

Maintainer
----------
Akiyoshi Kurita
FAS username: redadmin
GitHub: https://github.com/redadmin-k

For issues or suggestions, please open an issue or pull request.

