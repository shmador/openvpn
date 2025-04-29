# How to Use - OpenVPN Server Setup (Ubuntu)

1. Configure `inventory.ini` to match the remote server where you want to install the OpenVPN server

2. Run the playbook:

```bash
ansible-playbook -i inventory.ini playbook.yaml
```

This will create a `.ovpn` file that can connect to the remote server  
The IP in the file will match the host you set in `inventory.ini`

3. Use the generated config to connect:

```bash
sudo openvpn --config client.ovpn
```

You should now be connected via a VPN tunnel to the remote server

