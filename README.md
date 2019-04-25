# ansible-role-nginx-centos

Ansible role to install latest Nginx on CentOS

The role only install Nginx.
The role doesn't configure Nginx because it is difficult to configure Nginx generally and simply.
Some Ansible role (ex. [nginxinc.nginx](https://github.com/nginxinc/ansible-role-nginx) and [geerlingguy.nginx](https://github.com/geerlingguy/ansible-role-nginx)) configures Nginx but they are too complicated and learning cost is too high.

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
