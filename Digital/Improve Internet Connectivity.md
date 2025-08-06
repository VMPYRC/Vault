---
created: 2025-07-22
modified: 2025-07-22
description: 
aliases: 
tags:
  - Digital
---

# Instructions

1. Start Menu
2. Search for `Command Prompt`
3. Run as Administrator
4. Should open to `C:\Windows\System32>`
5. Enter the commands below

|                       Command                       | Note                                                                                                   |
| :-------------------------------------------------: | ------------------------------------------------------------------------------------------------------ |
|                   `sfc /scannow`                    | - scans and repairs corrupted or missing system files using the System File Checker                    |
| `netsh int tcp set global autotuninglevel=disabled` | - disables TCP auto-tuning                                                                             |
|        `netsh int ip reset c:\resetlog.txt`         | - resets all TCP/IP network settings to default and logs changes to `c:\resetlog.txt`                  |
|               `netsh int ipv6 reset`                | - resets IPv6 config (if you're using IPv6 and having issues)                                          |
|             `netsh int tcp show global`             | - displays current TCP settings                                                                        |
|                `netsh winsock reset`                | - resets the Winsock Catalog                                                                           |
|                 `ipconfig /release`                 | - releases the current IP address assigned to the device (disconnects it from the network temporarily) |
|                  `ipconfig /renew`                  | - requests a new IP address from the DHCP server (reconnects to the network)                           |
|                `ipconfig /flushdns`                 | - clears the DNS resolver cache, which can fix issues related to outdated or incorrect DNS entries     |
|                    `netstat -an`                    | - displays active connections and listening ports (good for spotting suspicious connections)           |
|               `ping [hostname or IP]`               | - checks if a target host is reachable and measures response time<br>- `ping duckduckgo.com`           |
