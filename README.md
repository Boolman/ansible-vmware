ansible-galaxy collection install -r collections.yaml

ansible-playbook -i input.json playbook.yaml



input.json:
```
{
  "all": {
    "hosts": {
      "foobar": {
        "vcenter_username": "user",
        "vcenter_password": "password.",
        "vcenter_hostname": "1.2.3.4",
        "datastore": "ds1",
        "datacenter": "dc1",
        "cluster": "dc1-cluster1",
        "folder": "my folder",
        "template_name": "my_template",
        "networks": [
          {
            "name": "vlan_name_001",
            "ip": "10.0.0.2",
            "netmask": "255.255.255.0",
            "gateway": "10.0.0.1",
            "dswitch_name": "DSwitch",
            "dns_servers": [ "8.8.8.8" ]
          }
	]
      }
    }
  }
}
```
