//==============================================================================
// ASIX AX88772B Windows XP driver
//
// This document describes the driver's configurable parameters.
//==============================================================================

1. Connection Type: Set the Ethernet link speed.
   -AutoSense:              Auto detect the Ethernet link speed
   -10BaseT Half_Duplex:    Set the Ethernet works on 10HD
   -10BaseT Full_Duplex:    Set the Ethernet works on 10FD
   -100BaseTx Half_Duplex:  Set the Ethernet works on 100HD
   -100BaseTx Full_Duplex:  Set the Ethernet works on 100FD

2. Network Address : Allows user to set a MAC address of the device or use the 
                     device default address.

3. Flow Control: Configure flow control advertised capabilities
   -Disabled            Disable flow control
   -Tx Enabled          Enable transmit flow control
   -Rx Enabled          Enable receive flow control
   -Rx & Tx Enabled     Enable transmit and receive flow control

4. VLAN ID: If user set a valid VLAN ID, the driver inserts the VLAN tag with 
            this VLAN ID into the transmit packets and device will filter the
            received packets.

5. Wake Up: Enable or disable the WOL ability

   -Disabled                      Disable the WOL ability
   -Link Change                   Wake up the computer when device detects
                                  Ethernet link Change
   -Magic Packet                  Wake up the computer when device receives
                                  a Magic Packet
   -Wake-Up Frame                 Wake up the computer when device receives
                                  a packet that matches a specified pattern
   -Link Change/Magic Packet      Allow link Change and Magic Packet to wake up
                                  the computer
   -Link Change/Wake-Up Frame     Allow link Change and Wake-Up Frame to wake up
                                  the computer
   -Magic Packet/Wake-Up Frame    Allow Magic Packet and Wake-Up Frame to wake
                                  up the computer
   -All                           Allow link Change, Magic Packet, and Wake-Up
                                  Frame to wake up the computer

6. Wake-Up Frame Type: Select the Wake-Up Frame patterns
   -Windows Default    Use the Wake-up frame patterns provided by Windows
   -PING               Use the PING Wake-up frame patterns
   -ARP                Use the ARP Wake-up frame patterns
   -PING/ARP           Use the PING and ARP Wake-up frame patterns

7. TCP Checksum Offload (IPv4): Enable or disable the device to calculate the
                                TCP checksum of the transmit IPv4 packets and
                                check the TCP checksum of the received IPv4
                                packets.
   -Disabled          Disable the TCP Checksum Offload
   -Tx Enabled        Enable the TCP Checksum Offload for transmit packets
   -Rx Enabled        Enable the TCP Checksum Offload for received packets
   -Rx & Tx Enabled   Enable the TCP Checksum Offload for transmit and received
                      packets

8. UDP Checksum Offload (IPv4): Enable or disable the device to calculate the
                                UDP checksum of the transmit IPv4 packets and
                                check the UDP checksum of the received IPv4
                                packets.
   -Disabled          Disable the UDP Checksum Offload
   -Tx Enabled        Enable the UDP Checksum Offload for transmit packets
   -Rx Enabled        Enable the UDP Checksum Offload for received packets
   -Rx & Tx Enabled   Enable the UDP Checksum Offload for transmit and received
                      packets

9. TCP Checksum Offload (IPv6): Enable or disable the device to calculate the
                                 TCP checksum of the transmit IPv6 packets and
                                 check the TCP checksum of the received IPv6
                                 packets.
    -Disabled          Disable the TCP Checksum Offload
    -Tx Enabled        Enable the TCP Checksum Offload for transmit packets
    -Rx Enabled        Enable the TCP Checksum Offload for received packets
    -Rx & Tx Enabled   Enable the TCP Checksum Offload for transmit and received
                       packets

10. UDP Checksum Offload (IPv6): Enable or disable the device to calculate the
                                 UDP checksum of the transmit IPv6 packets and
                                 check the UDP checksum of the received IPv6
                                 packets.
    -Disabled          Disable the UDP Checksum Offload
    -Tx Enabled        Enable the UDP Checksum Offload for transmit packets
    -Rx Enabled        Enable the UDP Checksum Offload for received packets
    -Rx & Tx Enabled   Enable the UDP Checksum Offload for transmit and received 
                       packets

11. IPv4 Checksum Offload: Enable or disable the device to calculate the IP 
                           checksum of the transmit IPv4 packets and check the
                           IP checksum of the received IPv4 packets.
    -Disabled           Disable the IP Checksum Offload
    -Tx Enabled         Enable the IP Checksum Offload for transmit packets
    -Rx Enabled         Enable the IP Checksum Offload for received packets
    -Rx & Tx Enabled    Enable the IP Checksum Offload for transmit and received
                        packets

12. AutoDetach: Enable or disable AutoDetach ability. if AutoDetach is enabled, 
                3 seconds later after Ethernet cable was unpluged, the device will
                be de-attached from USB.
    -Disabled           Disable AutoDetach
    -Enabled            Enable AutoDetach
    -Use EEPROM Setting Disable or enable AutoDetach accoring to the EEPROM setting.

13. Mask WakeUp Event Timer: If wake up ability is enabled, the wake up function
                             will delay this time to active.
        -0,4,8,12,16,20,24,28 seconds

14. WOL Link Speed: Set the Ethernet link speed when device sleeps if wake up 
                    ability is enabled.
    -10 Mbps First       The Ethernet link speed works on 10 Mbps first if available
    -Use EEPROM Setting  Use EEPROM setting to set Ethernet link speed

