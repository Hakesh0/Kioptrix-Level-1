# Kioptrix Level 1 - Enumeration

## Discovering the IP Address
- **arp-scan -l**: Use `arp-scan` to list all connected devices on the local network.

### Explanation
- **arp-scan**: ARP scanning tool that sends ARP requests and displays the responses, allowing you to discover devices on the local network.

## Discovering the IP Address (Alternate Method)
- **netdiscover -r 192.168.30.0/24**: Use `netdiscover` to discover devices on the network within the specified IP range.

### Explanation
- **netdiscover**: Network scanning tool that sends packets on the network and listens for responses, helping you discover devices within a specified IP range.
