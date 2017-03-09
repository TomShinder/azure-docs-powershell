---
external help file: Microsoft.Azure.Commands.ServiceBus.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzureRmServiceBusTopic

## SYNOPSIS
Gets a description for the specified Service Bus topic.

## SYNTAX

```
Get-AzureRmServiceBusTopic [-ResourceGroup] <String> [-NamespaceName] <String> [[-TopicName] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmServiceBusTopic** cmdlet gets a topic description for the specified Service Bus namespace.

## EXAMPLES

### Example 1: Get the description of the specified topic for a Service Bus namespace
```
PS C:\> Get-AzureRmServiceBusTopic -ResourceGroup "Default-ServiceBus-WestUS" -NamespaceName "SB-Example1" -TopicName "SB-Topic_example1"
```

This command gets the description of the specified topic for the given Service Bus namespace.

## PARAMETERS

### -NamespaceName
Specifies the name of the Service Bus namespace.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroup
Specifies the name of the resource group.

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

### -TopicName
Specifies the name of the Service Bus topic.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### -ResourceGroup
 System.String
 

### -NamespaceName
 System.String
 

### -TopicName
 System.String

## OUTPUTS

### Microsoft.Azure.Commands.ServiceBus.Models.TopicAttributes
Name                                : SB-Topic_exampl1
Location                            : West US
Id                                  : /subscriptions/854d368f-1828-428f-8f3c-f2affa9b2f7d/resourceGroups/Default-ServiceBus-WestUS/providers/Microsoft.ServiceBus/namespaces/SB-Example1/topics/S
                                      B-Topic_exampl1
Type                                : Microsoft.ServiceBus/Topic
AccessedAt                          : 1/20/2017 3:18:54 AM
AutoDeleteOnIdle                    : 10675199.02:48:05.4775807
EntityAvailabilityStatus            : 
CreatedAt                           : 1/20/2017 3:16:41 AM
CountDetails                        : Microsoft.Azure.Management.ServiceBus.Models.MessageCountDetails
DefaultMessageTimeToLive            : 10675199.02:48:05.4775807
DuplicateDetectionHistoryTimeWindow : 
EnableBatchedOperations             : True
EnableExpress                       : False
EnablePartitioning                  : True
EnableSubscriptionPartitioning      : False
FilteringMessagesBeforePublishing   : False
IsAnonymousAccessible               : False
IsExpress                           : False
MaxSizeInMegabytes                  : 16384
RequiresDuplicateDetection          : False
SizeInBytes                         : 0
Status                              : Active
SubscriptionCount                   : 1
SupportOrdering                     : False
UpdatedAt                           : 1/20/2017 3:16:43 AM

## NOTES

## RELATED LINKS

[New-AzureRmServiceBusTopic](./New-AzureRmServiceBusTopic.md)

[Remove-AzureRmServiceBusTopic](./Remove-AzureRmServiceBusTopic.md)

[Set-AzureRmServiceBusTopic](./Set-AzureRmServiceBusTopic.md)