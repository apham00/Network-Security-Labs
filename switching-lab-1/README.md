# Switching Lab

## Objective
Verify the default configuration of a Cisco Catalyst switch and configure basic VLAN interface settings.

## Topology
- 1 PC
- 1 Switch
- Console connection (PC → Switch)
- Ethernet connection (PC → FastEthernet0/1)
<img src="./switching.png" alt="Switching lab topology" width="600">

## Learned
- Connected the PC to the switch console port
- Connected the PC to FastEthernet0/1
- Accessed the switch through the terminal
- Entered privileged EXEC mode
- Checked the default switch configuration
- Viewed VLAN and interface information
- Configured VLAN 1 with an IP address
- Enabled the interface using `no shutdown`
- FastEthernet0/1 does not have an IP address because it is a Layer 2 switch port. On a switch, IP addresses are assigned to VLAN interfaces, such as VLAN 1, for management purposes.
<img src="./lab%201%20config.png" alt="Switch configuration screenshot" width="600">

## Key Commands
enable<br>
show running-config<br>
show startup-config<br>
show vlan brief<br>
show ip interface brief<br>
interface vlan 1<br>
ip address 192.168.1.2 255.255.255.0<br>
no shutdown<br>
