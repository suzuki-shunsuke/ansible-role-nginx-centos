# ansible-role-nginx-centos

[![GitHub last commit](https://img.shields.io/github/last-commit/suzuki-shunsuke/ansible-role-nginx-centos.svg)](https://github.com/suzuki-shunsuke/ansible-role-nginx-centos)
[![GitHub tag](https://img.shields.io/github/tag/suzuki-shunsuke/ansible-role-nginx-centos.svg)](https://github.com/suzuki-shunsuke/ansible-role-nginx-centos/releases)
[![License](http://img.shields.io/badge/license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/suzuki-shunsuke/ansible-role-nginx-centos/master/LICENSE)

Ansible role to install latest Nginx on CentOS

https://galaxy.ansible.com/suzuki-shunsuke/nginx_centos

The role only install Nginx.
The role doesn't configure Nginx because it is difficult to configure Nginx generally and simply.
Some Ansible roles (ex. [nginxinc.nginx](https://github.com/nginxinc/ansible-role-nginx) and [geerlingguy.nginx](https://github.com/geerlingguy/ansible-role-nginx)) configure Nginx but they are too complicated and learning cost is too high.

## Role Variables

https://github.com/suzuki-shunsuke/ansible-role-nginx-centos/blob/master/defaults/main.yml

## Dependencies

Nothing.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: suzuki-shunsuke.nginx_centos
      nginx_started: true
      become: true
```

## License

[MIT](LICENSE)
