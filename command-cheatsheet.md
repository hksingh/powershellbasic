# Command Basic
    >> Verb-Noun
    >> Do something - To get something

## Parameters 
    -ComputerName, -File, -Definition, -Name, 

## Verbs get-verb | more
> Add, Clear, Close, Copy, Enter, Exit
  Find, Get, Format, Join, New, Push, Open, Search, Show, Select, Split

## Verbs want to know more about the Verb like Set
> get-verb -Verb Set | more
> get-verb -Verb Set | format-list

# Get all verbs in Group Security :  Get-Verb | Where-Object Group -EQ Security

# Get all verbs start https://aka.ms/psverbs

# Get all aliases in powershell : get-alias |format-list
## Get alias first 5 :  get-alias | select -first 5
## Get alias Definition Security :  get-alias -Definition *select*

### gsv -Name D*   gets the service whose name starts with D

