# demo-compose
demo tools docker-compose

---

## quick start new vm(sample ubuntu)

``` bash

$ apt-get update

$ apt-get install docker.io

$ curl -L "https://github.com/docker/compose/releases/download/v2.20.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

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

## sample opensuse

``` bash
 $ zypper remove docker \
                  docker-client \
                  docker-client-latest \
                  docker-common \
                  docker-latest \
                  docker-latest-logrotate \
                  docker-logrotate \
                  docker-engine \
                  runc
 $ opensuse_repo="https://download.opensuse.org/repositories/security:/SELinux/openSUSE_Factory/security:SELinux.repo"
 $ sudo zypper addrepo $opensuse_repo
```
---
suse install docker 
``` bash
dnf config-manager --add-repo=https://download.docker.com/linux/centos/docker-ce.repo
dnf install docker-ce
systemctl enable --now docker


curl -L "https://github.com/docker/compose/releases/download/2.26.1/docker-compose-$(uname -s)-$(uname -m)" -o docker-compose
mv docker-compose /usr/local/bin && sudo chmod +x /usr/local/bin/docker-compose
ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```
