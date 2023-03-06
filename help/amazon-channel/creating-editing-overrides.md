---
title: Create and Edit Overrides
description: Use Amazon Sales Channel overrides to apply your changes to a single Amazon listing, or to multiple listings.
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
---
# Create and Edit Overrides

You can create and override for a listing or edit or remove an override that has been applied to a listing. Overrides set a defined value for a specific listing.

## Create an override for a single listing

The _[!UICONTROL Create Override]_ action is available when viewing listings on the _[!UICONTROL Inactive]_, _[!UICONTROL Active]_, and _[!UICONTROL Ineligible]_ tabs.

1. View a listing on a _[!UICONTROL Products Listings]_ page (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, and _[!UICONTROL Ineligible]_ tab).

1. In the _[!UICONTROL Action]_ column, click **[!UICONTROL Select]** > **[!UICONTROL Create Override]** to open the Product Listing Overrides page.

   ![create Amazon listing override](assets/amazon-select-create-override.png)

1. To ensure you are viewing the correct listing, verify the _[!UICONTROL Listing Details]_.

1. Determine the type of override you are creating.

   You can define a single override type or any combination of types for the listing (Price, Handling Time, Condition, Seller Notes).

   - **Price** - Click **[!UICONTROL Change Listing Price]** and enter your defined price value for **[!UICONTROL Price Override]**.
   - **Handling Time** - Click **[!UICONTROL Change Handling Time]** and enter the defined time value (in days) for **[!UICONTROL Handling Time Override]**.
   - **Condition** - Click **[!UICONTROL Change Condition]** and choose the correct option for the **[!UICONTROL Condition Override]**.
   - **Seller Notes** - Click **[!UICONTROL Change Seller Notes]** and enter your notes text for **[!UICONTROL Seller Notes Override]**.

1. Click **[!UICONTROL Save Listing Override]**.

    The _[!UICONTROL Product Listing Overrides]_ page closes. The status of the listing changes to `Relist in Progress`. The change will be published to Amazon with your next data sync (as configured in your cron settings). The listing is also added to the _[!UICONTROL Overrides]_ tab.

The following example shows an override that defines a new price of `$55`, a new handling time of `1 day`, a new condition of `Used; Like New`, and new Seller Note text.

![Example Amazon listing override](assets/amazon-overrides-edit.png)

## Edit or remove an override for a single listing {#edit-override-single-listing}

The _[!UICONTROL Edit Overrides]_ action is available when viewing listings on the _[!UICONTROL Overrides]_ tab.

1. View a listing on the _[!UICONTROL Product Listings]_ page (_[!UICONTROL Overrides]_ tab).

1. In the _[!UICONTROL Action]_ column, click **[!UICONTROL Select]** > **[!UICONTROL Edit Overrides]**.

   The _[!UICONTROL Product Listing Overrides]_ page opens.

    ![Select an Amazon listing override](assets/amazon-select-edit-overrides.png)

1. To ensure you are overriding the correct listing, verify the _[!UICONTROL Listing Details]_.

1. To edit your _[!UICONTROL Override]_ settings, define the sections for the type you want to change (Price, Handling Time, Condition, Seller Notes).

    To keep an override type the same, select `No Change To <override type>` (the default). This setting leaves the previously defined override value unchanged.

   - **Price** - Click **[!UICONTROL Change Listing Price]** and enter your defined price value for **[!UICONTROL Price Override]**.
   - **Handling Time** - Click **[!UICONTROL Change Handling Time]** and enter the defined time value (in days) for **[!UICONTROL Handling Time Override]**.
   - **Condition** - Click **[!UICONTROL Change Condition]** and choose the correct option for **[!UICONTROL Condition Override]**.
   - **Seller Notes** - Click **[!UICONTROL Change Seller Notes]** and enter your notes text for **[!UICONTROL Seller Notes Override]**.

1. To remove an override type, click **Remove** for each of the types you want to remove. If not removed, the previously defined value remains in the override.

1. Click **[!UICONTROL Save Listing Override]**.

    The _[!UICONTROL Product Listing Overrides]_ page closes. The status of the listing changes to `Relist in Progress`. The change will be published to Amazon with your next data sync (as configured in your cron settings). If not already listed, the listings are also added to the _[!UICONTROL Overrides]_ tab.

Piggybacking on the _Create an Override_ example. The following example shows an edit to the previously created override that defines a new price of `$50`, removes the Handling Time override, and keeps the previous Condition and Seller Notes overrides.

![Editing or removing an override](assets/amazon-overrides-edit-2.png)
__

## Edit or remove an override for multiple listings {#edit-override-multiple-listings}

The _[!UICONTROL Edit Listing Overrides]_ action is available on the _[!UICONTROL Inactive]_, _[!UICONTROL Active]_, _[!UICONTROL Overrides]_, and _[!UICONTROL Ineligible]_ tabs.

>[!NOTE]
>
>Because you are modifying overrides for multiple listings, the _[!UICONTROL Listing Details]_ section does not display as it does when modifying a single listing.

1. View the listing on a _[!UICONTROL Products Listings]_ page (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, _[!UICONTROL Overrides]_, and _[!UICONTROL Ineligible]_ tab).

1. Select the checkbox in the left-side column for each of the listings you want to modify.

1. Under _[!UICONTROL Actions]_, click **[!UICONTROL Edit Listing Overrides]**.

   The _[!UICONTROL Product Listing Overrides]_ page opens.

    ![Select an Amazon listing override](assets/amazon-actions-edit-listing-overrides.png)

1. To edit your _[!UICONTROL Override]_ settings, define the sections for the type you want to change (Price, Handling Time, Condition, Seller Notes).

    To keep an override the same, select `No Change To <override type>` (default). This setting leaves the previously defined override value unchanged.

   - **Price** - Click **[!UICONTROL Change Listing Price]** and enter your defined price value for **[!UICONTROL Price Override]**.
   - **Handling Time** - Click **[!UICONTROL Change Handling Time]** and enter the defined time value (in days) for **[!UICONTROL Handling Time Override]**.
   - **Condition** - Click **[!UICONTROL Change Condition]** and choose the correct option for **[!UICONTROL Condition Override]**.
   - **Seller Notes** - Click **[!UICONTROL Change Seller Notes]** and enter your notes text for **[!UICONTROL Seller Notes Override]**.

1. To remove an override type, click **[!UICONTROL Remove]** for each of the types you want to remove. If not removed, the previously defined value remains in the override.

1. Click **[!UICONTROL Save Listing Override]**.

    The _[!UICONTROL Product Listing Overrides]_ page closes. The status of the listings changes to `Relist in Progress`. The change will be published to Amazon with your next data sync (as configured in your cron settings). If not already listed, the listings are also added to the _[!UICONTROL Overrides]_ tab.

### Override types

|Override|Description|
|--- |--- |
|[!UICONTROL Price Override]|A price override defines the price for the listings. This override takes priority over all automated settings until the override is removed.<br><br>To override the price of your product, choose **[!UICONTROL Change Listing Price]** and enter the new price for **[!UICONTROL Price Override]**. |
|[!UICONTROL Handling Time Override]|A handling time override defines the time it takes (in days) to process and ship products. A handling time override takes priority over all automated and default handling time settings until the override is removed.<br><br>The value that exists in the _[!UICONTROL Handling Time Override]_ box is either your default handling time defined in your [listing settings](./listing-settings.md) or your defined override handling time. If you remove a handling time override, the listing defaults to the handling time defined in your listing settings.<br><br>To define a handling time override, choose **[!UICONTROL Change Handling Time]** and enter the new handling time (in days) for **[!UICONTROL Handling Time Override]**. |
|[!UICONTROL Condition Override]|To override the Listing Condition, choose **[!UICONTROL Change Condition]** and choose the new condition from **Condition Override**. |
|[!UICONTROL Seller Notes Override]|For products in your catalog that are defined with a condition other than `New`, a seller note can be added to further detail your product and its condition to potential buyers. You can enter a seller note override for a `New` condition product, but Amazon does not display the note.<br><br>To override the Seller Notes, choose **[!UICONTROL Change Seller Notes]** and enter the new note for **[!UICONTROL Seller Notes Override]**.|
