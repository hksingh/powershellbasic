## use outputFormatters
> Format-Table  Format-List 
## using the pipe symbol : Write powershell command from single line to multiple line 
> get-service |   
 where-Object Status -eq 'Stopped'

### use where-object / select-object to choose where and select to select
>get-service |
 where-Object Status -eq 'Stopped' |
 select-object name, status, displayname

### Store result in a variable.
> $result = get-service | where-Object Status -eq 'Stopped'| select-object name, status, displayname

### out-file select-object first 5 and output to a file 
> get-service |
>> where-object Status -eq 'Stopped' |
>> select-object Status, Name, DisplayName |
>> select-object -First 5 | out-file .\services.csv

### get total # of commands
>(get-command).count

### get versions : $PSVersionTable

### search with wildchar :  Get-Service "sh*"  

### sort-object : Get-Service "s*" | Sort-Object displayname