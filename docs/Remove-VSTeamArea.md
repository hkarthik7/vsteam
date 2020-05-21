---
external help file: VSTeam-Help.xml
Module Name: VSTeam
online version:
schema: 2.0.0
---

# Remove-VSTeamArea

## SYNOPSIS

Removes an existing area from the project


## SYNTAX

## DESCRIPTION

Removes an existing area from the project


## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------

```PowerShell
PS C:\> Remove-VSTeamArea -ProjectName Demo -Path "\MyIteration\Path"
```

This command removes an existing area with the path MyIteration/Path to the Demo project. Any work items that are assigned to that path get reassigned to the root area, since no reclassification id has been given.

### -------------------------- EXAMPLE 2 --------------------------

```PowerShell
PS C:\> Remove-VSTeamArea -ProjectName "Demo" -Path "\MyIteration\Path" -ReClassifyId 19
```

This command removes an existing area with the path \MyIteration\Path to the Demo project. Any work items that are assigned to that path get reassigned to the area with the id 19.

## PARAMETERS

### -ProjectName

Specifies the team project for which this function operates.

You can tab complete from a list of available projects.

You can use Set-VSTeamDefaultProject to set a default project so
you do not have to pass the ProjectName with each call.

```yaml
Type: String
Position: 0
Required: True
Accept pipeline input: true (ByPropertyName)
```

### -Path

Path of the area node.

```yaml
Type: string
```

### -ReClassifyId

Id of an area where work items should be reassigned to if they are currently assigned to the area being deleted.

```yaml
Type: int
```

### -Force

Forces the function without confirmation

```yaml
Type: SwitchParameter
Required: false
Position: Named
Accept pipeline input: false
Parameter Sets: (All)
```

## INPUTS

## OUTPUTS

### System.Object

## NOTES

This function is a wrapper of the base function Remove-VSTeamClassificationNode.md.

## RELATED LINKS

[Remove-VSTeamClassificationNode](Remove-VSTeamClassificationNode.md)

[Remove-VSTeamIteration](Remove-VSTeamIteration.md)
