# Kioptrix Level 1 - SMB Enumeration and Connection

## MSFconsole SMB Enumeration

### Overview
- **Purpose**: MSFconsole is used for reconnaissance, exploiting vulnerabilities, and delivering payloads.
- **Command**: `msfconsole`

### Search for SMB Version
- **Command**: `search smb`
- **Purpose**: Searches for the version of the SMB service running on the target machine.

### Use SMB Version Auxiliary Module
- **Command**: `use auxiliary/scanner/smb/smb_version`
- **Purpose**: Uses the SMB version auxiliary module to retrieve the version of the SMB service.

### Set RHOSTS and Run
- **Command**: 
  ```
  set RHOSTS 192.168.30.128
  run
  ```
- **Purpose**: Sets the target host IP address and runs the module to obtain the SMB version information.

## SMB Client Connection

### Overview
- **Purpose**: SMBclient is used to connect to SMB shares as an anonymous user.
- **Command**: `smbclient -L \\\\192.168.30.128\\` (or `smbclient -L \\192.168.30.128`)
- **Purpose**: Lists the available SMB shares on the target machine.

### Connect to Specific SMB Share
- **Command**: 
  ```
  smbclient \\\\192.168.30.128\\ADMIN$
  smbclient \\\\192.168.30.128\\IPS$
  ```
- **Purpose**: Attempts to connect to the specified SMB shares on the target machine.

You can save this content in a Markdown file in your repository and update your README.md file to include this new file. Let me know if you need any more help!
```
