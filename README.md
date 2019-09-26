cloud3rsio.selinux
=========

Update selinux setting.

Installation
------------

```bash
$ ansible-galaxy install cloud3rsio.selinux
```

Requirements
------------

Nothing.

Role Variables
--------------

Nothing.
| Key | Default Value | Type | Comment |
| ------------- | ------------- | ------------- | ------------- |
| `selinux_policy` | `targeted` | String | If you use Enforcing or Permissive. |

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
# Enforcing
- hosts: all
  roles:
    - role: cloud3rsio.selinux/enforcing

# Permissive
- hosts: all
  roles:
    - role: cloud3rsio.selinux/permissive
      selinux_policy: minimum

# Disabled
- hosts: all
  roles:
    - role: cloud3rsio.selinux/disabled
```

License
-------

[MIT](LICENSE)

Author Information
------------------

- youyo
