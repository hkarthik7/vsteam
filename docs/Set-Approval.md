---
external help file: Team-Help.xml
Module Name: 
online version: 
schema: 2.0.0
---

# Set-Approval

## SYNOPSIS
Sets the status of approval to Approved, Rejected, Pending, or ReAssigned.

## SYNTAX

```
Set-Approval [-ProjectName] <String> [-Id] <Int32[]> [-Status] <String> [[-Approver] <String>]
 [[-Comment] <String>] [-Force]
```

## DESCRIPTION
Set-Approval sets the status of approval to Approved, Rejected, Pending, or ReAssigned.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Approval | Set-Approval
```

This command sets all pending approvals to approved.

### -------------------------- EXAMPLE 2 --------------------------
```
Set-Approval -Id 1 -Status Rejected
```

This command rejects approval with Id of 1.

## PARAMETERS

### -ProjectName
Specifies the team project for which this function operates.

You can tab complete from a list of available projects.

You can use Set-DefaultProject to set a default project so
you do not have to pass the ProjectName with each call.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Id
Specifies the approval IDs of the approvals to set.

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Status
Specifies the status to set for the approval.

Valid values: 'Approved', 'Rejected', 'Pending', 'ReAssigned'

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: Approved
Accept pipeline input: False
Accept wildcard characters: False
```

### -Approver
Specifies the user to whom the approval has been re-assigned to
Alias of the user.
chuckreinhart@outlook.com, for example.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Comment
Specifies the comment to be stored with this approval.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Sets the status without prompting for confirmation.

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

## INPUTS

### System.Int32[]
System.String

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS
