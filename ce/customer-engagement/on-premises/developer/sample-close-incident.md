---
title: "Sample: Close an incident (Developer Guide for Dynamics 365 Customer Engagement (on-premises)) | MicrosoftDocs"
description: "The sample code demonstrates how to process and close an incident (case) with a case resolution."
ms.custom: 
ms.date: 10/01/2019
ms.reviewer: 
ms.service:
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: samples
applies_to: 
  - Dynamics 365 Customer Engagement (on-premises)
helpviewer_keywords: 
  - processing and closing incidents (cases), service entities sample
  - sample for closing incidents (cases)
ms.assetid: 748ac902-3ba5-456c-ab91-aece8947131a
author: KumarVivek
ms.author: kvivek
manager: annbe
search.audienceType: 
  - developer
search.app: 
  - D365CE
---
# Sample: Close an incident

This sample code is for Dynamics 365 Customer Engagement (on-premises). [Download the Service samples](https://code.msdn.microsoft.com/Service-Samples-f42adf82).   

## Prerequisites
[!INCLUDE[sdk-prerequisite](../includes/sdk-prerequisite.md)]
  
## Requirements  
[!INCLUDE[sdk_SeeConnectionHelper](../includes/sdk-seeconnectionhelper.md)]
  
## Demonstrates  
 This sample shows how to process and close an incident (case) with a case resolution.  
  
## Example  
 [!code-csharp[Service#CloseAnIncident](../snippets/csharp/CRMV8/service/cs/closeanincident.cs#closeanincident)]  
  
### See also  
 [Incident (Case) Entities](incident-case-entities.md)   
 <xref:Microsoft.Crm.Sdk.Messages.CloseIncidentRequest>   
 <xref:Microsoft.Crm.Sdk.Messages.IsValidStateTransitionRequest>
