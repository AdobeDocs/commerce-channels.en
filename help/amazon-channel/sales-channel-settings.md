---
title: Sales Channel Settings
description: To manage logging, cron source, and synchronization for Amazon sales channel functions, update the Commerce configuration.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
---
# Sales Channel Settings

When the [!DNL Amazon Sales Channel] extension is installed, default values are set in the Admin for Amazon sales channel. These settings can be modified in your configuration settings for your Amazon store. These settings include:

- Intervals for clearing Activity Log history
- Cron source selection
- Log synchronization options

## Modify the Commerce channels settings

1. On the _Admin_ sidebar, go to **[!UICONTROL Stores]** > _[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**.

1. In the left panel, expand **[!UICONTROL Sales Channels]** and choose **[!UICONTROL Global Settings]**.

1. For **[!UICONTROL Clear Log History]**, choose an option:

   - `Once Daily` - Choose to clear your store activity history once daily.

   - `Once Weekly` - Choose to clear your store activity history once weekly.

   - `Once Monthly` - (Default) Choose to clear your store activity history once monthly.

1. For **[!UICONTROL Background Tasks (CRON) Source]**, choose `Magento CRON`.

   This option allows Amazon sales channel to use your [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) settings to determine communication and data sync intervals with [!DNL Amazon Seller Central].

1. For **[!UICONTROL Enable Debug Logging]**, choose `Enabled` to collect additional synchronization data when troubleshooting is needed.

   Amazon sales channel logging is written to the `{Commerce Root}/var/log/channel_amazon.log` file and can be viewed in [developer mode](https://docs.magento.com/user-guide/magento/installation-modes.html){target="_blank"}. Logging should only be `Enabled` during troubleshooting and should be `Disabled` when troubleshooting is complete.

1. For **[!UICONTROL Read-Only Mode]**, select `Enabled` to block all outgoing state-changing API requests.
   
   With this setting, potential changes are saved, but not sent, until [!UICONTROL Read-Only Mode] is disabled. The configuration cache must be cleared for Read-Only Mode to enable. To start the data transfers again, select `Disabled`. 

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] is designed for copies of the Production instance, such as staging or QA, and should not be used on the production instance.
   >
   >When a database is migrated to a new copy of the instance (detected when a store's URL changes in the configuration), [!UICONTROL Read-Only Mode] is automatically enabled.

1. Click **[!UICONTROL Save Config]**.

![Sales Channel configuration settings](assets/config-sales-channel-global-settings.png)
