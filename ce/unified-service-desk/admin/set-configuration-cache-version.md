---
title: "Cache specific configuration for agents in Unified Service Desk  | MicrosoftDocs"
description: "Learn how Cache specific configuration for agents in the configuration of Unified Service Desk ."
ms.custom: 
  - dyn365-USD
  - dyn365-admin
ms.date: 04/10/2019
ms.service: dynamics-365-customerservice
ms.topic: article
ms.assetid: A988412D-5A59-42BC-B608-0FB4E7CA7E17
author: kabala123
ms.author: kabala
manager: shujoshi
search.audienceType: admin
search.app: 
  - D365CE
  - D365USD
monikerRange: '>= dynamics-usd-4.1'
---

# Cache specific configuration for agents

The Configuration Cache Version option causes the client caching feature to retrieve the configuration that has undergone change from the Customer Engagement server to the agent’s desktop and avoid retrieving all configurations.

Your organization may have several departments and a each department has a configuration with agents added to those configurations. Whenever you make a change to one of those configurations, the **Configuration Cache Version** feature helps to download only that specific configuration for which you've made a change. Also, when the agents assigned to other configurations, sign in to the client application, the feature doesn't download the configurations thus improves the startup time of Unified Service Desk. This is also helpful in better application life cycle management for Unified Service Desk in cases where your organization want to make changes in your pilot or developer configurations without impacting the production users.

> [!div class=mx-imgBorder]
> ![Configuration Cache Version option in new configuration page with an example value](../media/configuration-cache-version.PNG "Configuration Cache Version option with an example value")

## Overview of Configuration Cache Version

Your organization has multiple configurations, and you’ve added agents to those configurations. Now, you make certain changes to any one configuration and update the **ClientCacheVersionNumber** in the server.

The next time the agent signs in to the Unified Service Desk client application, the client caching feature retrieves the configuration data from the Customer Engagement server for all the configurations even though you made the change to only one configuration. Retrieving multiple configurations can cause an increase in startup time, which in turn might degrade the startup performance.

To avoid retrieving all configurations from the Customer Engagement server when it’s not needed for every configuration, use the **Configuration Cache Version** option.

## What is Configuration Cache Version

**Configuration Cache Version** is an option on the **Configuration** page in the Unified Service Desk Customer Engagement server settings. Every configuration in the Unified Service Desk in the Customer Engagement server has the **Configuration Cache Version** option and takes an alphanumeric value as the cache key.

## How does Configuration Cache Version work
The following scenario example explains how Configuration Cache Version works.

> [!div class=mx-imgBorder]
> ![1 update configuration x, 2 agent signs in to Unified Service Desk, 3 client caching verifies the key, and 4. downloads the configuration x from server to agent desktop](../media/ccv-working.GIF "Configuration Cache version working")

Your organization uses **X**, **Y**, and **Z** configurations for chat, message, and voice support, respectively. You make a change to configuration X and update the **Configuration Cache Version** value in the server. When an agent assigned to configuration **X** (chat) signs in to the Unified Service Desk client application, the client caching feature checks for the local cache store and determines the cache version key. Because you updated the cache version key for the **Configuration Cache Version** option, the client caching feature retrieves the updated configuration **X** from the server to the agent’s desktop.

## Enable the Configuration Cache Version option

> [!div class=mx-imgBorder]
> ![In the new option page, add EnableConfigurationCaching for name and enter value as true](../media/configuration-cache-version.GIF "EnableConfigurationCaching UII option with value as true")

1. Sign in to the Common Data Service platform.

2. Select the down arrow next to Dynamics 365.

3. Select **Unified Service Desk Administrator**.

4. Select **Options** under **Advance Settings** in the site map.

5. Select **New** on the **Active UII Options** page.

6. Select **Others** for **Global Option**, enter **EnableConfigurationCaching** in the Name box, and enter **true** in the value box.

7. Select **Save**.

Unified Service Desk activates the client caching for configurations.

## Specify value for the Configuration Cache Version option

1. Sign in to the Common Data Service platform.

2. Select the down arrow next to Dynamics 365.

3. Select **Unified Service Desk Administrator**.

4. Select **Configuration** under **Advance Settings** in the site map.

5. Select an existing configuration from the list or create a new configuration.

6. Enter an alphanumeric value as the cache key in the text box of the **Configuration Cache Version** field on the **Configuration** page. For example, the alphanumeric value can be updated as **XY12**.

7. Select **Save**.

## Client caching store location
When enabled, client caching stores its files in a compressed and encrypted format in the user’s roaming directory: `%appData%\Microsoft\Microsoft Dynamics 365 Unified Service Desk`

For example, for a user called agent1 running the Unified Service Desk client application on Windows 8, the client caching files are available at `c:\Users\agent1\AppData\Roaming\Microsoft\Microsoft Dynamics 365 Unified Service Desk`.


## See also

[Configure client caching in Unified Service Desk](configure-client-caching-unified-service-desk.md)

[Manage access using Unified Service Desk configuration](manage-access-using-unified-service-desk-configuration.md)
