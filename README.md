OULibraries.nfs-server
=========

NFS Server for OULib.

Requirements
------------

A target system running CentOS7x.

Role Variables
--------------

```
nfs_shares:
  - path: /srv/share1
    clients:
      - ip: 192.168.1.10
        perms: ['rw','sync','no_root_squash','all_squash']
      - ip: 192.168.1.11
        perms: ['rw','sync','no_root_squash','all_squash']
  - path: /srv/share2
    clients:
      - ip: 192.168.1.0/24
        perms: ['rw','sync','no_root_squash','all_squash']

```
and so forth.

Dependencies
------------


Example Playbook
----------------


License
-------

TBD

Author Information
------------------

Jason Sherman
