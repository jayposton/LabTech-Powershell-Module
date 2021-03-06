# Invoke-LTServiceCommand
## SYNOPSIS
This function tells the agent to execute the desired command.
## SYNTAX
```powershell
Invoke-LTServiceCommand [-Command] <String[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```
## DESCRIPTION
This function will allow you to execute all known commands against an agent.
## PARAMETERS
### -Command &lt;String[]&gt;

```
Required                    true
Position                    2
Default value
Accept pipeline input       true (ByValue)
Accept wildcard characters  false
```
### -WhatIf &lt;SwitchParameter&gt;

```
Required                    false
Position                    named
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Confirm &lt;SwitchParameter&gt;

```
Required                    false
Position                    named
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## NOTES
Version:        1.2

Author:         Chris Taylor

Website:        labtechconsulting.com

Creation Date:  2/2/2018

Purpose/Change: Initial script development

Thanks:         Gavin Stone, for finding the command list



Update Date: 2/8/2018

Purpose/Change: Updates for better overall compatibility, including better support for PowerShell V2



Update Date: 3/21/2018

Purpose/Change: Removed ErrorAction Override 
