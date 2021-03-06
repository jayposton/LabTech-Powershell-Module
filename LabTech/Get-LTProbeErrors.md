# Get-LTProbeErrors
## SYNOPSIS
This will pull the %ltsvcdir%\LTProbeErrors.txt file into an object.
## SYNTAX
```powershell
Get-LTProbeErrors [<CommonParameters>]
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Get-LTProbeErrors | where {(Get-date $_.Time) -gt (get-date).AddHours(-24)}

Get a list of all errors in the last 24hr
```

### EXAMPLE 2
```powershell
PS C:\>Get-LTProbeErrors | Out-Gridview

Open the log file in a sortable searchable window.
```

## NOTES
Version:        1.1

Author:         Chris Taylor

Website:        labtechconsulting.com

Creation Date:  3/14/2016

Purpose/Change: Initial script development



Update Date: 6/1/2017

Purpose/Change: Updates for better overall compatibility, including better support for PowerShell V2



Update Date: 3/18/2018

Purpose/Change: Changed Erroraction from Stop to unspecified to allow caller to set the ErrorAction. 
