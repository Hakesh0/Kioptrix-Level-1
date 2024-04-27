
# Kioptrix Level 1 - SSH Connection and Vulnerability Research

## SSH Connection Attempt

- **Command**: 
  ```bash
  ssh 192.168.30.128
  ```
- **Issue**: Unable to negotiate with 192.168.30.128 port 22: no matching key exchange method found. Their offer: diffie-hellman-group-exchange-sha1,diffie-hellman-group1-sha1
- **Recommendation**: Try using the following command to specify a key exchange algorithm:
  ```bash
  ssh 192.168.30.128 -oKexAlgorithms=+diffie-hellman-group-exchange-sha1
  ```

## Vulnerability Research

- **Purpose**: Find potential vulnerabilities of all the ports found using nmap.
- **Action**:
  - Search in Google or use `$searchsploit Samba2`.
  - Port 80/443 - Potentially vulnerable to OpenLuck:
    - [ExploitDB](https://www.exploit-db.com/exploits/764)
    - [GitHub](https://github.com/heltonWernik/OpenLuck)
  - Port 139 - Potentially vulnerable to trans2open:
    - [Rapid7](https://www.rapid7.com/db/modules/exploit/linux/samba/trans2open/)
    - [ExploitDB](https://www.exploit-db.com/exploits/10)
```
