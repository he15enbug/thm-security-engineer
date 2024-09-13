# Network and System Security

## Secure Network Architecture

### Network Segmentation

- Let’s consider a scenario where a client brings in their own device, a common practice known as BYOD (Bring Your Own Device). The client’s device was infected with a Remote Access Trojan (RAT) that will attempt to traverse the network the device is connected to and exfiltrate any sensitive information. With subnetting in place, there is no restriction in place as to where the infected device could connect as long as the proper routes are in place, leaving sensitive information and servers open to the unknown device. How do we fix this problem? VLANs!
- **VLANs** (**V**irtual **LAN**) are used to segment portions of a network at **layer two** and differentiate devices.
- VLANs are configured on a switch by adding a "tag" to a frame. The 802.1q or dot1q tag will designate the VLAN that the traffic originated from.
- The 802.1 tag provides a standard between vendors that will always define the VLAN of a frame. For example, if our switches are Cisco and our routers are Juniper, they can send tagged frames and digest them equally because it is standardized.
