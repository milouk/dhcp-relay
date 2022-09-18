This is a dhcp relay using the dhcp-helper.


## How to use

Add the following service to your docker-compose file

```
dhcphelper:
  image: milouk/dhcp-helper
  restart: always
  network_mode: host
  command: -s <Your PiHole Bridge Network IP>
  cap_add:
   - NET_ADMIN
```
