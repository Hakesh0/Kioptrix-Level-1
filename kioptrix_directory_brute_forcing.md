# Kioptrix Level 1 - Directory Brute Forcing

## DirBuster
- **Command**: `dirbuster& (paste: http://192.168.30.128:80/ - port is important)`
- **Result**: 
  - While DirBuster is running, open Burp Suite and try to find server information.
  - After DirBuster is complete, enumerate all the files and try to find information.

## Why it's used
- DirBuster is used to find all possible files and directories on the target machine, which can help identify hidden or unlinked content that may be accessible.
