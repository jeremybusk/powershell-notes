# powershell-notes

https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_try_catch_finally?view=powershell-7

## Linting Style checking
```
Install-Module -Name PSScriptAnalyzer
Invoke-ScriptAnalyzer myscript.ps1
```

```
Get-WinEvent -LogName *PowerShell*, Microsoft-Windows-Kernel-WHEA* |
  Group-Object -Property LevelDisplayName, LogName -NoElement |
    Format-Table -AutoSize
```
