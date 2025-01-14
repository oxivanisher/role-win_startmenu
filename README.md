win_startmenu
=============

Configure Start menu related settings:
* Disable app succestions
* Disable bing search
* Disable "tip" popup (Ads)
* Disable copilot

Requirements
------------

This role is built to be used with Ansible oder SSH on Windows.

Role Variables
--------------

| Name                                | Comment                        | Default value |
|-------------------------------------|--------------------------------|---------------|
| win_startmenu_users                 | List of users to be configured | `[Default]`   |
| win_startmenu_also_for_ansible_user | Also configure `ansible_user`  | `true`        |

Example Playbook
----------------
```yaml
- name: Configure the Windows Start menu
  hosts: windows
  roles:
    - role: oxivanisher.windows_desktop.win_startmenu
```
License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.windows_desktop](https://galaxy.ansible.com/ui/repo/published/oxivanisher/windows_desktop/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-windows_desktop).
