# Kioptrix Level 1 - Port Scanning

## Scanning for Open Ports
- **nmap -T4 -p- -A 192.168.30.128**: Use `nmap` to perform a thorough scan with aggressive options, including scanning all ports and enabling OS detection, version detection, script scanning, and traceroute.

### Explanation
- **nmap**: Network scanning tool that scans for open ports and services on a target machine.
- **-T4 (Timing Template)**: Sets the timing of the scan to be more aggressive, speeding up the scan process.
- **-p- (Port Specification)**: Specifies that all ports should be scanned, from port 1 to the maximum port number.
- **-A (Aggressive Scan Options)**: Enables additional advanced scanning techniques, including OS detection, version detection, script scanning, and traceroute.
