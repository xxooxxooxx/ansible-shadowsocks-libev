# ansible-shadowsocks-libev
[![Build Status](https://travis-ci.org/xxooxxooxx/ansible-shadowsocks-libev.svg?branch=master)](https://travis-ci.org/xxooxxooxx/ansible-shadowsocks-libev)

### Debian 8+/CentOS 7+ ansible 2.3+
* init
```
ssh-keygen -t ed25519 -C "name"
ssh-keygen -E md5 -lf ~/.ssh/ansible_id_ed25519.pub
ssh-copy-id -i ~/.ssh/ansible_id_ed25519.pub root@ip

eval "$(ssh-agent -s)"
ssh-add ~/.ssh/ansible_id_ed25519
ssh-add -l -E md5

```
* /etc/ansible/hosts
```
[ss]
#ssh-agent
1.2.3.4 ansible_user=root
5.6.7.8 ansible_user=root ansible_ssh_private_key_file=/root/.ssh/ansible_id_ed25519
#CentOS 8
9.10.11.12:99 ansible_python_interpreter=/usr/bin/python3 ansible_user=root ansible_ssh_pass='2Hc?5!F4JSeU1zzk'
```
