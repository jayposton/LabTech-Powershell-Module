# Test-LTPorts
## SYNOPSIS
This function will attempt to connect to all required TCP ports.
## SYNTAX
```powershell
Test-LTPorts [[-Server] <String[]>] [[-TrayPort] <Int32>] [-Quiet] [<CommonParameters>]
```
## DESCRIPTION
The function will confirm the LTTray port is available locally.
It will then test required TCP ports to the Server.
## PARAMETERS
### -Server &lt;String[]&gt;
This is the URL to your LabTech server. 

Example: https://lt.domain.com

If no server is provided the function will use Get-LTServiceInfo to 

get the server address. If it is unable to find LT currently installed 

it will try calling Get-LTServiceInfoBackup.
```
Required                    false
Position                    1
Default value
Accept pipeline input       true (ByValue, ByPropertyName)
Accept wildcard characters  false
```
### -TrayPort &lt;Int32&gt;
This is the port LTSvc.exe listens on for communication with LTTray.

It will be checked to verify it is available. If not provided the 

default port will be used (42000).
```
Required                    false
Position                    2
Default value                0
Accept pipeline input       true (ByPropertyName)
Accept wildcard characters  false
```
### -Quiet &lt;SwitchParameter&gt;
This will return a boolean for connectivity status to the Server
```
Required                    false
Position                    named
Default value                False
Accept pipeline input       true (ByPropertyName)
Accept wildcard characters  false
```
## NOTES
Version:        1.6

Author:         Chris Taylor

Website:        labtechconsulting.com

Creation Date:  3/14/2016

Purpose/Change: Initial script development



Update Date:    5/11/2017 

Purpose/Change: Quiet feature



Update Date: 6/1/2017

Purpose/Change: Updates for better overall compatibility, including better support for PowerShell V2



Update Date: 6/10/2017

Purpose/Change: Updates for pipeline input, support for multiple servers



Update Date: 8/24/2017

Purpose/Change: Update to use Clear-Variable.



Update Date: 8/29/2017

Purpose/Change: Added Server Address Format Check



Update Date: 2/13/2018

Purpose/Change: Added -TrayPort parameter. 
