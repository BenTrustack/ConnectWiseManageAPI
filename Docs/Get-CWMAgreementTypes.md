---
external help file: ConnectWiseManageAPI-help.xml
Module Name: ConnectWiseManageAPI
online version: https://developer.connectwise.com/Products/ConnectWise_PSA/REST#/AgreementTypes/getFinanceAgreementsTypes
schema: 2.0.0
---

# Get-CWMAgreementTypes

## SYNOPSIS
This function will list agreement types based on conditions.

## SYNTAX

```
Get-CWMAgreementTypes [-id <Int32>] [-count] [[-condition] <String>] [[-orderBy] <String>]
 [[-childConditions] <String>] [[-customFieldConditions] <String>] [[-page] <Int32>] [[-pageSize] <Int32>]
 [-fields <String[]>] [-all] [<CommonParameters>]
```

## DESCRIPTION
{{ Fill in the Description }}

## EXAMPLES

### EXAMPLE 1
```powershell
Get-CWMAgreementTypes -Condition "company/identifier=`"$($Config.company.identifier)`"
```

Will list the agreement types that match the condition.

## PARAMETERS

### -all
Return all results

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -childConditions
Allows searching arrays on endpoints that list childConditions under parameters

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

### -customFieldConditions
Allows searching custom fields when customFieldConditions is listed in the parameters

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

### -orderBy
Choose which field to sort the results by, 'field/sub desc' or 'field/sub asc'

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -page
Used in pagination to cycle through results

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 4
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -pageSize
Number of results returned per page (Defaults to 25)

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: 5
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -fields
Allows you to return a partial response with just the fields listed.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -id
{{ Fill id Description }}

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -count
Will return the number of objects.

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

### -condition
This is your search condition to return the results you desire.
Example: `(contact/name like "Fred%" and closedFlag = false) and dateEntered \> \[2015-12-23T05:53:27Z\] or summary contains "test" AND  summary != "Some Summary"`

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Author: Chris Taylor Date: 04/10/2023

## RELATED LINKS

[https://developer.connectwise.com/Products/ConnectWise_PSA/REST#/AgreementTypes/getFinanceAgreementsTypes](https://developer.connectwise.com/Products/ConnectWise_PSA/REST#/AgreementTypes/getFinanceAgreementsTypes)
