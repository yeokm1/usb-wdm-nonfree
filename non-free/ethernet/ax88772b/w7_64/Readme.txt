//==============================================================================
// ASIX AX88772B Windows 7 driver
//
// This document describes the driver's configurable parameters.
//==============================================================================

1. Speed & Duplex: Set the Ethernet link speed.
   -Auto Negotiation:              Auto detect the Ethernet link speed
   -10 Mbps Half Duplex:    Set the Ethernet works on 10HD
   -10 Mbps Full Duplex:    Set the Ethernet works on 10FD
   -100 Mbps Half Duplex:   Set the Ethernet works on 100HD
   -100 Mbps Full Duplex:   Set the Ethernet works on 100FD

2. Network Address : Allows user to set a MAC address of the device or use the 
                     device default address.

3. Flow Control: Configure flow control advertised capabilities
   -Disabled            Disable flow control
   -Tx Enabled          Enable transmit flow control
   -Rx Enabled          Enable receive flow control
   -Rx & Tx Enabled     Enable transmit and receive flow control

4. Packet Priority & VLAN: Enable or disable the ability to insert the 802.1Q
                           priority and VLAN tags into the transmit packets.
   -Packet Priority & VLAN Disable Disable to insert the 802.1Q priority and VLAN tag
   -Packet Priority Enable         Only enable to insert the 802.1Q priority tag
   -VLAN Enable                    Only enable to insert the 802.1Q VLAN tag
   -Packet Priority & VLAN Enable  Enable to insert the 802.1Q priority and VLAN tag

5. VLAN ID: If user set a valid VLAN ID, the driver inserts the VLAN tag with 
            this VLAN ID into the transmit packets and device will filter the
            received packets.

6. Wake on link change: Enable or disable the device to wake up the computer 
			when detects the Ethernet link Change
   -Disabled		Disable the Wake on link change
   -Enabled		Enable the Wake on link change

7. Wake on Magic Packet: Enable or disable the device to wake up the computer 
			when receives a magic packet
   -Disabled		Disable the Wake on Magic Packet
   -Enabled		Enable the Wake on Magic Packet

8. Wake on pattern match: Enable or disable the device to wake up the computer 
			when receives a matched wakeup pattern
   -Disabled		Disable the Wake on pattern match
   -Enabled		Enable the Wake on pattern match

9. TCP Checksum Offload (IPv4): Enable or disable the device to calculate the
                                TCP checksum of the transmit IPv4 packets and
                                check the TCP checksum of the received IPv4
                                packets.
   -Disabled          Disable the TCP Checksum Offload
   -Tx Enabled        Enable the TCP Checksum Offload for transmit packets
   -Rx Enabled        Enable the TCP Checksum Offload for received packets
   -Rx & Tx Enabled   Enable the TCP Checksum Offload for transmit and received
                      packets

10. UDP Checksum Offload (IPv4): Enable or disable the device to calculate the
                                UDP checksum of the transmit IPv4 packets and
                                check the UDP checksum of the received IPv4
                                packets.
   -Disabled          Disable the UDP Checksum Offload
   -Tx Enabled        Enable the UDP Checksum Offload for transmit packets
   -Rx Enabled        Enable the UDP Checksum Offload for received packets
   -Rx & Tx Enabled   Enable the UDP Checksum Offload for transmit and received
                      packets

11. TCP Checksum Offload (IPv6): Enable or disable the device to calculate the
                                 TCP checksum of the transmit IPv6 packets and
                                 check the TCP checksum of the received IPv6
                                 packets.
    -Disabled          Disable the TCP Checksum Offload
    -Tx Enabled        Enable the TCP Checksum Offload for transmit packets
    -Rx Enabled        Enable the TCP Checksum Offload for received packets
    -Rx & Tx Enabled   Enable the TCP Checksum Offload for transmit and received
                       packets

12. UDP Checksum Offload (IPv6): Enable or disable the device to calculate the
                                 UDP checksum of the transmit IPv6 packets and
                                 check the UDP checksum of the received IPv6
                                 packets.
    -Disabled          Disable the UDP Checksum Offload
    -Tx Enabled        Enable the UDP Checksum Offload for transmit packets
    -Rx Enabled        Enable the UDP Checksum Offload for received packets
    -Rx & Tx Enabled   Enable the UDP Checksum Offload for transmit and received 
                       packets

13. IPv4 Checksum Offload: Enable or disable the device to calculate the IP 
                           checksum of the transmit IPv4 packets and check the
                           IP checksum of the received IPv4 packets.
    -Disabled           Disable the IP Checksum Offload
    -Tx Enabled         Enable the IP Checksum Offload for transmit packets
    -Rx Enabled         Enable the IP Checksum Offload for received packets
    -Rx & Tx Enabled    Enable the IP Checksum Offload for transmit and received
                        packets

14. ARP Offload: When enable this ability, the device will reply the ARP request
                 packet when computer is suspending. This ability is activated only
                 if WOL is enabled.
    -Disabled           Disable ARP Offload
    -Enabled            Enable ARP Offload

15. NS Offload: When enable this ability, the device will reply the neighbor
                solicitation packet when computer is suspending. This ability is 
                activated only if WOL is enabled.
    -Disabled           Disable NS Offload
    -Enabled            Enable NS Offload

16. AutoDetach: Enable or disable AutoDetach ability. if AutoDetach is enabled, 
                3 seconds later after Ethernet cable was unpluged, the device will
                be detached from USB.
    -Disabled           Disable AutoDetach
    -Enabled            Enable AutoDetach
    -Use EEPROM Setting Disable or enable AutoDetach accoring to the EEPROM setting

17. Mask WakeUp Event Timer: If wake up ability is enabled, the wake up function
                             will delay this time to active.
        -0,4,8,12,16,20,24,28 seconds

18. WOL Link Speed: Set the Ethernet link speed when device sleeps if wake up 
                    ability is enabled.
    -10 Mbps First       The Ethernet link speed works on 10 Mbps first if available
    -Use EEPROM Setting  Use EEPROM setting to set Ethernet link speed
