This ansible role will help you copy config for yandex-tank to docker host, and run it.

Put this role to your roles folder, and invoke it as follows:

```
- hosts: somehost

  vars:
    tank_configs_path: files/tank
    tank_load_ini: aws-m3xlarge.ini
    tank_host_path: /var/data/tank/
    tank_docker_name: aws-m3xlarge-test

  roles:
    - tank
```
