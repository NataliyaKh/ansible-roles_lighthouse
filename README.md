Role Name
=========

Install NGINX if needed, deploy [Lighthouse](https://github.com/VKCOM/lighthouse) GUI using ansible.

Requirements
------------

* Ansible >= 2.17

* Python >= 3.10.12

* Jinja >= 3.0.3

(It might work on previous versions, but we cannot guarantee it)


Role Variables
--------------

| Scope    | Variable            | Default                                 | Description                   |
|----------|---------------------|-----------------------------------------|-------------------------------|
| defaults | lighthouse_vcs      | https://github.com/VKCOM/lighthouse.git | Lighthouse repository address |
| defaults | lighthouse_location | /var/www/lighthouse                     | Installation destination      |

Dependencies
------------

- 

Example Playbook
----------------

```
    - name: Install Lighthouse
      hosts: lighthouse
      become: true
      roles:
        - lighthouse-role
      tags: lighthouse
```

License
-------

MIT

Author Information
------------------

Nataliya Khanova
