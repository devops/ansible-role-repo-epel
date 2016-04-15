# Ansible Role: repo-epel

Configure EPEL Repo for RedHat/CentOS.

## Requirements

repo_epel_baseurl和repo_epel_mirrorlist同时只能设置一个.

## Role Variables

`defaults/main.yml`

* `repo_epel_rpm: True`
* `repo_epel_baseurl: ""`
* `repo_epel_mirrorlist: ""`
* `repo_epel_backup: no`


## Dependencies

None.

## Example Playbook

    - name: Install epel repo.
      hosts: servers
      roles:
        - role: ansible-role-repo-epel
          repo_epel_rpm: False
          repo_epel_baseurl: http://mirrors.ustc.edu.cn/epel/7/x86_64/

## License

MIT / BSD

## Author Information

z
