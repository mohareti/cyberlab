---
title: "Powershell"
permalink: /docs/13_Powershell_101/
toc: true
excerpt: " The central repository for sharing and acquiring PowerShell code including PowerShell modules, scripts, and DSC resources. [Powershell Gallery](https://www.powershellgallery.com/) ."
tags:
  - powershell
  - powershell-gallery
  - package-management
published: true
# header:
#   teaserlogo:
#   teaser: ''
#   image: ''
#   caption:
gallery:
  - image_path: ''
    url: ''
    title: ''

---

{% include toc title="Table of content" %}
> The central repository for sharing and acquiring PowerShell code including PowerShell modules, scripts, and DSC resources. [Powershell Gallery](https://www.powershellgallery.com/) .

# Introduction
-  PowerShell is based on Microsoft .NET
- PowerShell editors: Visual Studio Code (VS Code)[http://code.visualstudio.com], PowerShell Studio, and PowerShell ISE
# Version

# Consoles
1. PowerShell Console
2. PowerShell ISE
  - used to write scripts
3. Elevated Console
4. x86 Console
  - 32-bit, legacy systems

# Cmdlets
- start-Transcript
- Get-Command
- Get-Command -Noun service
- Control + c to start
- Verb-Noun -parameters pattern
- Get-Help
 - pdate-Help
- new-item  -item-type
- dir | measure
- help Get-Date
- Get-Help Get-Date
- Get_help Get-Date Examples
- get-help get-date -online
- Get-Help *service*
- Get-Service
- Stop-Service  
- Start_service
- show-command get-service
- measure-commnad { }
- get-help new-item -ShowWindow
- copy-item path destination
- Get-Content
- Get-ChildItem  -Recurse
- Get-PsDrive
- get-item
- where-Object
- Get-Member -MemberType
- get-history
- select-object
- foreach-object
- write-host
- count
- Tee-Object
- write-error
- write-warning
- write-debug




# Alias
- cls
- get-alias cls
- get-process
- get-process -Name Mircrosoft | Get-Member
- select-object *

# Variables

- $name =

# coparison
- gt

# Lopping
- ForEach-Object
- ForEach-object {intialization }{loop }{end statement}

# colors
- Foregroundcolor red

# Passwords with PowerShell

''' PowerShell
$username
$plain_passwd = ''
$secure_passwd = $plain_passwd | ConvertTo-SecureString -AsPlainText -Force
$plainCred = New-Object system.management.automation.pscredential -ArgumentList $username, $secure_passwd


# Event Log
- Get-EventLog System -after (get-date).AddMinutes(-1000)
- assigning date
  - $Assign_Date =Get-Date 4/5/2010 8:00 PM
- Get-Date $Assign_Date -Format MMMM
- Get-Date $Assign_Date -Format MM
- Get-Date $Assign_Date -Format MMM
- Get-Date $Assign_Date -Format d
- Get-Date $Assign_Date -Format dddd
- Get-Date $Assign_Date -Format "MMMM dd, yyyy"
- 'M' for moths, 'm' for minutes

# write-Host
