# openvpn

OpenVPN server configuration role  
Handles everything — just run the `.ovpn` file (it will appear in the directory where the playbook is run)

---

## Requirements

- Remote Ubuntu machine

---

## Role Variables

- `server_ip` – No need to configure, it is set automatically to match the remote Ansible host

---

## Dependencies

None

---

## Example Playbook

```yaml
- hosts: servers
  become: yes
  roles:
    - openvpn
```

---

## License

BSD

---

## Author Information

Dor Attar  
dorattar4@gmail.com  
[GitHub - shmador](https://github.com/shmador)

