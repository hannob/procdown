procdown
========

Harden access to the `/proc` filesystem in Linux.

This script restricts read access to some files in the Linux `/proc` filesystem that may
enable attacks or leak private information.

recommendations
---------------

`/proc` should be mounted with the `hidepid=2` or `hidepid=invisible` option to prevent
user processes from being visible to other users.

The kernel option `CONFIG_SECURITY_DMESG_RESTRICT` prevents kernel messages from being
visible to unprivileged users.

author
------

This script was written by [Hanno Böck](https://hboeck.de/).
