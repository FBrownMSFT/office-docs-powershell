---
applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016
schema: 2.0.0
---

# Remove-WebServicesVirtualDirectory

## SYNOPSIS
!!! Exchange Server 2010

Use the Remove-WebServicesVirtualDirectory cmdlet to remove an existing virtual directory from a computer running Microsoft Exchange Server 2010 that has the Client Access server role installed.

!!! Exchange Server 2013

This cmdlet is available only in on-premises Exchange.

Use the Remove-WebServicesVirtualDirectory cmdlet to remove an existing virtual directory from a computer running Microsoft Exchange Server 2013.

For information about the parameter sets in the Syntax section below, see Exchange cmdlet syntax (https://technet.microsoft.com/library/bb123552.aspx).

!!! Exchange Server 2016

This cmdlet is available only in on-premises Exchange.

Use the Remove-WebServicesVirtualDirectory cmdlet to remove existing Exchange Web Services virtual directories from Internet Information Services (IIS) on Microsoft Exchange servers.

For information about the parameter sets in the Syntax section below, see Exchange cmdlet syntax (https://technet.microsoft.com/library/bb123552.aspx).

## SYNTAX

```
Remove-WebServicesVirtualDirectory [-Identity] <VirtualDirectoryIdParameter> [-Confirm]
 [-DomainController <Fqdn>] [-Force] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
!!! Exchange Server 2010

You can remove the default Exchange Web Services virtual directory or another Exchange Web Services virtual directory.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Exchange Web Services settings" entry in the Client Access Permissions topic.

!!! Exchange Server 2013

You can remove the default Exchange Web Services virtual directory or another Exchange Web Services virtual directory.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Exchange Web Services virtual directory settings" entry in the Clients and mobile devices permissions topic.

!!! Exchange Server 2016

You can remove the default Exchange Web Services virtual directory or another Exchange Web Services virtual directory.

You need to be assigned permissions before you can run this cmdlet. Although this topic lists all parameters for the cmdlet, you may not have access to some parameters if they're not included in the permissions assigned to you. To find the permissions required to run any cmdlet or parameter in your organization, see Find the permissions required to run any Exchange cmdlet (https://technet.microsoft.com/library/mt432940.aspx).

## EXAMPLES

### Example 1 -------------------------- (Exchange Server 2010)
```
Remove-WebServicesVirtualDirectory -Identity CAS01\Sales
```

This example removes the virtual directory Sales from the server CAS01.

### Example 1 -------------------------- (Exchange Server 2013)
```
Remove-WebServicesVirtualDirectory -Identity CAS01\Sales
```

This example removes the virtual directory Sales from the server CAS01.

### Example 1 -------------------------- (Exchange Server 2016)
```
Remove-WebServicesVirtualDirectory -Identity MBX01\Sales
```

This example removes the Exchange Web Services virtual directory named Sales from the server named MBX01.

## PARAMETERS

### -Identity
!!! Exchange Server 2010, Exchange Server 2013

The Identity parameter specifies a virtual directory.



!!! Exchange Server 2016

The Identity parameter specifies Exchange Web Services virtual directory that you want to remove.

You can use any value that uniquely identifies the virtual directory. For example:

- Name or \<Server\>\\Name

- Distinguished name (DN)

- GUID

The Name value uses the syntax "\<VirtualDirectoryName\> (\<WebsiteName\>)" from the properties of the virtual directory. You can specify the wildcard character (\*) instead of the default website by using the syntax \<VirtualDirectoryName\>\*.



```yaml
Type: VirtualDirectoryIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016

Required: True
Position: 1
Default value: None
Accept pipeline input: True
Accept wildcard characters: False
```

### -Confirm
The Confirm switch specifies whether to show or hide the confirmation prompt. How this switch affects the cmdlet depends on if the cmdlet requires confirmation before proceeding.

- Destructive cmdlets (for example, Remove-\* cmdlets) have a built-in pause that forces you to acknowledge the command before proceeding. For these cmdlets, you can skip the confirmation prompt by using this exact syntax: -Confirm:$false.

- Most other cmdlets (for example, New-\* and Set-\* cmdlets) don't have a built-in pause. For these cmdlets, specifying the Confirm switch without a value introduces a pause that forces you acknowledge the command before proceeding.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DomainController
The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.

```yaml
Type: Fqdn
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
!!! Exchange Server 2010

The Force parameter specifies whether to force the command to execute without asking for user confirmation. If set to $true, this parameter forces the command to execute without asking for user confirmation.



!!! Exchange Server 2013

The Force switch specifies whether to force the command to execute without asking for user confirmation. If set to $true, this parameter forces the command to execute without asking for user confirmation.



!!! Exchange Server 2016

The Force switch specifies whether to suppress warning or confirmation messages. You can use this switch to run tasks programmatically where prompting for administrative input is inappropriate. You don't need to specify a value with this switch.



```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
The WhatIf switch simulates the actions of the command. You can use this switch to view the changes that would occur without actually applying those changes. You don't need to specify a value with this switch.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  
To see the input types that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Input Type field for a cmdlet is blank, the cmdlet doesn't accept input data.

## OUTPUTS

###  
To see the return types, which are also known as output types, that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Output Type field is blank, the cmdlet doesn't return data.

## NOTES

## RELATED LINKS

[Online Version](https://technet.microsoft.com/library/ae2ac9a4-1951-4176-baa6-06839cdd64a0.aspx)
