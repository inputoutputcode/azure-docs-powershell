---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: e9cf2266-b5c7-4274-a5f4-46dced7278cc
schema: 2.0.0
ms.assetid: 2E8CD4D6-DAD9-4BFF-B318-077F756B0073
---

# Remove-AzureVMDscExtension

## SYNOPSIS
Removes an Azure DSC extension from a virtual machine.

## SYNTAX

```
Remove-AzureVMDscExtension -VM <IPersistentVM> [-Profile <AzureSMProfile>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureVMDscExtension** cmdlet removes an Azure DSC extension from a virtual machine.
The output of this cmdlet needs to be piped to the Update-AzureVM cmdlet.

## EXAMPLES

### Example 1: Remove a DSC extension from a virtual machine
```
PS C:\>Remove-AzureVMDscExtension -VM $VM | Update-AzureVM
```

This command removes an Azure DSC extension from a virtual machine.

## PARAMETERS

### -VM
Specifies the persistent virtual machine object.

```yaml
Type: IPersistentVM
Parameter Sets: (All)
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureVMDscExtension](./Get-AzureVMDscExtension.md)

[Set-AzureVMDscExtension](./Set-AzureVMDscExtension.md)

[Update-AzureVM](./Update-AzureVM.md)

