#include "./common/header.md"

# Remove-Build

## SYNOPSIS

## SYNTAX

```
Remove-Build [-ProjectName] <String> [-Id] <Int32[]> [-Force]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Build | Remove-Build -Force
```

This command will delete all builds that are not marked retain indefinitely.

## PARAMETERS

### -Id
Specifies one or more builds by ID.
To specify multiple IDs, 
use commas to separate the IDs.
To find the ID of a build,
type Get-Build.

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Force
Sets the status without prompting for confirmation.
By default, Remove-Build prompts for confirmation before removing
any build.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

#include "./params/projectName.md"

## INPUTS

### System.Int32[]
System.String

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS
