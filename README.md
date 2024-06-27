# Networking_pkt
a guided Cisco Packet Tracer project about GE_4ax SCADA Network

![alt text](https://github.com/jackDante/Networking_pkt/blob/main/GE.png)


 Where a single device like a pc, printer or server is connected to a port, then you should use "switchport mode access" and switchport access vlan xxx, where xxx is the vlan number.

```
SG350X#show vlan
SG350X#configure terminal
SG350X(config)#interface [interface-id | range vlan vlan-range]
SG350X(config-if-range)#switchport mode access
SG350X(config-if-range)#switchport access vlan [vlan-id | none]
(Optional) Per riassegnare la porta o l'intervallo di porte alla VLAN predefinita, immettere quanto segue: SG350X(config-if-range)#no switchport access vlan
SG350X(config-if-range)#exit
SG350X(config-if)#end
SG350X#show vlan
SG350X#copy running-config startup-config

SG350X#configure terminal
SG350X#interface [interface-id | range vlan vlan-range]
SG350X(config-if)#switchport mode trunk
SG350X(config-if)#switchport trunk allowed vlan [all | none | add vlan-list | remove vlan-list | except vlan-list]
```
## sw 1-2-3
https://www.cisco.com/c/en/us/support/switches/catalyst-ie3300-rugged-series/series.html

## sw backbone01
https://www.cisco.com/c/en/us/support/switches/catalyst-9500-series-switches/series.html
