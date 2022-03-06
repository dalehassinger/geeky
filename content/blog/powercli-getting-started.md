---
title: "PowerCLI Getting Started"
description: "description"
image: "images/post/powershell.png"
date: 2020-04-19T00:00:00-05:00
categories: ["PowerCLI"]
tags:
- PowerShell
- PowerCLI
type: "regular" # available types: [featured/regular]
draft: false
---

<div>
  <b>PowerCLI Basics</b>
</div>
<div>
  <br>
</div>


###### PowerCLI Code

Some basic PowerCLI commands


{{< highlight powershell >}}

#Here are some basic commands that you can keep adding additional code
#and get more precise on what you want to see.

#Connect to a vCenter

Connect-VIServer vcsa.domain.org

#Disconnect from vCenter and not be prompted

Disconnect-VIServer vcsa.domain.org -confirm:$false

#Get VM Listing

#Shows all VMs
Get-VM

#Shows all VMs sorted by Name
Get-VM | Sort-Object Name

#Shows all VMs sorted by Name that are Powered On
Get-VM | Where-Object {$_.Powerstate -eq 'PoweredOn'} | Sort-Object Name

#Shows all VMs sorted by Name, that are Powered On and only shows
#Name,MemoryGB,NumCpu
Get-VM | Where-Object {$_.Powerstate -eq 'PoweredOn'} | Sort-Object Name | Select-Object Name,MemoryGB,NumCpu

{{< /highlight >}}

