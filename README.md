# Qemu Kvm bridge debian 12
```
#The loopback network interface
auto lo
iface lo inet loopback

#The primary network interface
auto enp3s0
iface enp3s0 inet manual

#Configure bridge > Mac da placa principal 
auto br0
iface br0 inet dhcp
bridge_ports enp3s0
bridge_hw <MAC>

```
