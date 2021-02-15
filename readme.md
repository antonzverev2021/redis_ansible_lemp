# LEMP on Ubuntu 18.04

This playbook will install a LEMP environment on an Ubuntu 18.04 machine and Redis
## Settings

- `mysql_root_password`: the password for the MySQL root account.
- `http_host`: your domain name.
- `http_conf`: the name of the configuration file that will be created within nginx.
- `http_port`: HTTP port, default is 80.


## Running this Playbook

Quick Steps:

### 1.  Options

```shell
nano vars/default.yml
```

#vars/default.yml
---
#mysql_root_password: "mysql_root_password"
#http_host: "your_domain"
#http_conf: "your_domain.conf"
#http_port: "80"

### Running
```command
ansible-playbook -l [target] -i [inventory file] -u [remote user] playbook.yml
```

