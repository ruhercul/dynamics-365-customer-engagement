---
title: "Manage storage for Dynamics 365 for Customer Engagement apps (online) | MicrosoftDocs"
ms.custom: 
  - dyn365-deflc
ms.date: 05/30/2019
ms.reviewer: 
ms.service: crm-online
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
applies_to: 
  - Dynamics 365 for Customer Engagement  (online)
  - Dynamics 365 for Customer Engagement  Version 9.x
ms.assetid: cf4bf53e-4458-4fec-a837-aaa0e946d1ed
caps.latest.revision: 4
author: jimholtz
ms.author: jimholtz
manager: kvivek
search.audienceType: 
  - admin
search.app: 
  - D365CE
  - Powerplatform
---
# Manage storage 

> [!NOTE]
> Capacity reports are now available. See [Common Data Service storage capacity](https://docs.microsoft.com/power-platform/admin/capacity-storage). The content below applies to customers with capacity reports not yet available.

You can manage your organization’s data storage capacity in connection with your subscription to [!INCLUDE[pn_CRM_Online](../includes/pn-crm-online.md)] apps. The type of subscription you purchase determines the amount of storage initially allocated to your organization. If you run out of storage, you can add more.  
  
 You can also gain storage by deleting certain types of unnecessary data in Customer Engagement apps. For information on deleting data, see: [Free storage space in Dynamics 365 for Customer Engagement](free-storage-space.md).  
  
 For information on storage amounts included with the various [!INCLUDE[pn_CRM_Online](../includes/pn-crm-online.md)] apps plans, see: [Dynamics 365 for Customer Engagement apps pricing](https://www.microsoft.com/dynamics365/pricing).  
  
## Monitor the amount of storage your organization is using  

Most customers can now monitor storage usage in the [Power Platform Admin center](https://docs.microsoft.com/power-platform/admin/capacity-storage).
   
If you're a customer with a non-commercial subscription, such as Dynamics 365 for Customer Engagement for U.S. Government (Dynamics 365 GCC and GCC High), follow the steps below to view storage consumption.
  
If your total storage used is 80% or more of capacity, [!INCLUDE [pn-crm-shortest](../includes/pn-crm-shortest.md)] apps admins will receive email notifications and alerts will appear on the Service Health page.  
  
1. [!INCLUDE[proc_office365_signin](../includes/proc-office365-signin.md)]  
  
2. [!INCLUDE[proc_office365_choose_admin_crm](../includes/proc-office365-choose-admin-crm.md)]  
  
3. Choose the **Service Health** tab.  
  
   ![View storage consumed by each instance](../admin/media/instance-storage.png "View storage consumed by each instance")  

## Add storage to Dynamics 365 for Customer Engagement apps (online)  
 
As a global or billing administrator, you can purchase additional storage for your company on Microsoft 365 admin center by following the steps below. [Learn how to find your global or billing administrator](../basics/find-administrator-support.md). 

 Monitor your Customer Engagement apps storage to make sure you’ve got lots of capacity for growth.  
  
 If your total storage used is 80% or more of capacity, [!INCLUDE [pn-crm-shortest](../includes/pn-crm-shortest.md)] apps admins will receive email notifications and alerts will appear on the Service Health page.  
  
1. [!INCLUDE[proc_office365_signin](../includes/proc-office365-signin.md)]  
  
2. [!INCLUDE[proc_office365_choose_admin_crm](../includes/proc-office365-choose-admin-crm.md)]  
  
3. Choose the **Service Health** tab.  
  
   ![View storage consumed by each instance](../admin/media/instance-storage.png "View storage consumed by each instance")  

If you purchase through volume licensing or a cloud solutions provider, please contact your partner directly.  
 
1. [!INCLUDE[proc_office365_signin](../includes/proc-office365-signin.md)]  
  
2. Click **Billing** > **Purchase Services**.  
  
3. Scroll down to the **Add-on subscriptions** section and mouse over the **Dynamics 365 - Additional Database Storage** tile.  
  
   ![Purchase additional online storage](../admin/media/purchase-additional-online-storage.png "Purchase additional online storage")  
  
4. Click **Buy now**, and then proceed through the order process.  
  
     If you paid for the subscription by credit card, any additional storage space that you order will be available immediately after you receive an order confirmation. If you’re invoiced for subscription payments, you may be asked to complete a credit check. In this case, the additional storage will not be available until the credit check is passed.  

## What happens if you exceed your storage limit?

[!INCLUDE [pn-crm-shortest](../includes/pn-crm-shortest.md)] apps System administrators will receive frequent email notifications which will cease once additional storage is added or storage is reduced to below the limit.

### See also  
 [Manage Microsoft Dynamics 365 for Customer Engagement apps (online) instances](../admin/manage-online-instances.md)   
 [Free storage space in Microsoft Dynamics 365 for Customer Engagement](free-storage-space.md)   
 [Manage subscriptions, licenses, and user accounts](../admin/manage-subscriptions-licenses-user-accounts.md)   
 [Global and Service administrators can administer Dynamics 365 for Customer Engagement apps without a license](../admin/global-service-administrators-can-administer-without-license.md)
