---
title: journalLine resource type | Microsoft Docs
description: A journal line object in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.service: "dynamics365-business-central"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: solsen
---

# journalLine resource type
Represents a journal line in [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

> [!NOTE]  
> For information about enabling APIs for [!INCLUDE[navnow](../../includes/navnow_md.md)] see [Enabling the APIs for Dynamics 365 Business Central](../enabling-apis-for-dynamics-nav.md).

## Methods
| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET journalLine](../api/dynamics_journalLine_Get.md)|journalLine|Gets a journal line object.|
|[DELETE journalLine](../api/dynamics_journalLine_Delete.md)|none|Deletes a journal line object.|
|[POST journalLine](../api/dynamics_journalLine_Create.md)|journalLine|Creates a journal line object.|
|[PATCH journalLine](../api/dynamics_journalLine_Update.md)|journalLine|Updates a journal line object.|




## Navigation

| Navigation |Return Type| Description |    
|:----------|:----------|:-----------------|
|[journal](../resources/dynamics_journal.md)|journal |Gets the journal of the journalLine.|
|[customerPaymentJournal](../resources/dynamics_customerpaymentjournal.md)|customerPaymentJournal |Gets the customerpaymentjournal of the journalLine.|
|[account](../resources/dynamics_account.md)|account |Gets the account of the journalLine.|
|[attachments](../resources/dynamics_attachments.md)|attachments |Gets the attachments of the journalLine.|
|[dimensionSetLines](../resources/dynamics_dimensionsetlines.md)|dimensionSetLines |Gets the dimensionsetlines of the journalLine.|


## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the item. Non-editable.|
|journalId|GUID|The ID of the journal.|
|journalDisplayName|string|The display name of the journal that this line belongs to. Read-Only.|
|lineNumber|integer|The journal line item line number.|
|accountType|NAV.genJournalAccountType|Specifies the type of account. It can be "G/L Account", "Customer", "Vendor", "Bank Account", "Fixed Asset", "IC Partner" or "Employee".|
|accountId|GUID|The id of the account that the journal line is related to. |
|accountNumber|string|The number of the account that the journal line is related to. |
|postingDate|date|The date that the journal line   is posted.|
|documentNumber|string|Specifies a document number for the journal line.|
|externalDocumentNumber|string|Specifies an external document number for the journal line.|
|amount|decimal|Specifies the total amount (including VAT) that the journal line consists of.|
|description|string|Specifies the description of the journal line.|
|comment|string|A user specified comment on the journal line.|
|lastModifiedDateTime|datetime|The last datetime the journal line was modified. Read-Only.|


## JSON representation

Here is a JSON representation of the journalLine resource.


```json
{
   "id": "GUID",
   "journalId": "GUID",
   "journalDisplayName": "string",
   "lineNumber": "integer",
   "accountType": "NAV.genJournalAccountType",
   "accountId": "GUID",
   "accountNumber": "string",
   "postingDate": "date",
   "documentNumber": "string",
   "externalDocumentNumber": "string",
   "amount": "decimal",
   "description": "string",
   "comment": "string",
   "lastModifiedDateTime": "datetime"
}
```
## See also

[GET journalLine](../api/dynamics_journalLine_Get.md)   
[DELETE journalLine](../api/dynamics_journalLine_Delete.md)   
[POST journalLine](../api/dynamics_journalLine_Create.md)   
[PATCH journalLine](../api/dynamics_journalLine_Update.md)   
