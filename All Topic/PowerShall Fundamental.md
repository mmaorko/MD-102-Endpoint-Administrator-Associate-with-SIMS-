PowerShall Fundamental: PowerShall is powerfull command line shell and scripting language. which is maninly used for system administration and automation purpose 
- Purpose: Helps automate various administrative tasks on Windows systems—such as file management, service configuration, user account control, etc.
- Foundation: Built on the .NET Framework, and supports Object-Oriented scripting.
- Commands: PowerShell commands are called cmdlets, such as Get-Process, Set-Location, Get-Service, etc.

## Some basic command line
File System Navigation

| Command                              | Description                                  |
| ------------------------------------ | -------------------------------------------- |
| `Get-Location` or `pwd`              | Shows current directory                      |
| `Set-Location <path>` or `cd <path>` | Changes directory                            |
| `Get-ChildItem` or `ls`              | Lists files and folders in current directory |
| `Clear-Host` or `clear`              | Clears the PowerShell screen                 |


## System Information

| Command              | Description                                            |
| -------------------- | ------------------------------------------------------ |
| `Get-Process`        | Lists running processes                                |
| `Get-Service`        | Lists Windows services                                 |
| `Get-Date`           | Displays current date and time                         |
| `Get-Help <command>` | Shows help for a command (e.g. `Get-Help Get-Process`) |
