---
title: "Open Ports - Zero Trust"
description: "description"
image: "images/post/port-check.png"
date: 2021-04-24T00:00:00-05:00
categories: ["Zero Trust"]
tags:
- NSX
- PowerShell
- Zero Trust
- vRealize Suite
type: "regular" # available types: [featured/regular]
draft: false
---

<div>
  <b>How to check if ports are open to a remote server</b>
</div>

###### PowerShell Code

Use PowerShell to see if ports are open to a remote server.

Living in a zero trust environment can be challenging. Here is some code that I have been using to test for open ports from a Windows server to any type of destination. Just change PortNumber and Destination for your use case.

{{< highlight powershell >}}

# --- Is Port Open
$PortNumber = '443'
$ComputerName = 'Server.vCrocs.info'

$results = Test-NetConnection -ComputerName $ComputerName -Port $PortNumber

Write-host 'Computer Name:'$ComputerName
Write-host 'Port:'$PortNumber
Write-host 'Port Open:'$results.TcpTestSucceeded

{{< /highlight >}}

###### Linux Commands
If you work with VMware vRealize Suite of appliances here are some commands (curl and Netcat) that can be used with Linux OS to test if ports are open to destination servers.  

{{< highlight powershell >}}

curl -v telnet://server01.vCROCS.info:443
nc -ztv server01.vCROCS.info 443 -w 3

{{< /highlight >}}
