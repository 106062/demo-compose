# demo-compose
demo tools docker-compose

---

## quick start new vm(sample ubuntu)

``` bash

$ apt-get update

$ apt-get install docker.io

$ curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

$ chmod +x /usr/local/bin/docker-compose

$ ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose

// nvm
$ curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
$ source ~/.profile

// change timezone
$ timedatectl list-timezones
$ timedatectl set-timezone ${timezone}
```

## gitlab-ce default init password path

``` cmd
/etc/gitlab/initial_root_password
```
- [use LDAP](https://chrislee0728.medium.com/%E5%BB%BA%E7%BD%AE-gitlab-%E7%89%88%E6%8E%A7%E5%B7%A5%E5%85%B7-5fe047330e91)
