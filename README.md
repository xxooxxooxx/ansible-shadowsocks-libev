# ansible-shadowsocks-libev

### Debian 8+/CentOS 7+

* /etc/ansible/hosts
```
.
[ss]
1.2.3.4 ansible_ssh_private_key_file=/root/.ssh/ansible_id_ed25519
#5.6.7.8 (CentOS 8)
5.6.7.8:99 ansible_python_interpreter=/usr/bin/python3 ansible_ssh_pass='2Hc?5!F4JSeU1zzk'
.
```

```
ansible-playbook ss.yml
```