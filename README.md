Role Name
=========

This rule installs and configures wireguard-ui (https://github.com/ngoduykhanh/wireguard-ui).

Requirements
------------

This role requires wireguard to be installed. 

Role Variables
--------------

Required variables to be set on command-line or in the playbook are:

* wgui_username - Username to access the wireguard-ui
* wgui_password - Password to access the wireguard-ui

In `defaults/main.yaml` the following variables and default-values are specified.

```yaml
wg_ui_version: "0.3.6"
wg_ui_os: "linux"
wg_ui_architecture: "amd64"
```

Dependencies
------------

none

Example Playbook
----------------
This role can be easily used in a playbook like this: 

```yaml
- hosts: wireguard-server
  roles:
      - ansible-role-wgui
```

License
-------
GNU GENERAL PUBLIC LICENSE VERSION 3

Author Information
------------------
[blog.retter.jetzt](https://blog.retter.jetzt)