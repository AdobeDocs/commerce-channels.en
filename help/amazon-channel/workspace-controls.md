---
title: Workspace Controls
description: Amazon Sales Channel provides workspace controls help you locate listings, view information, and easily and apply actions.
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
---
# Workspace controls

The Amazon sales channel [home page](./amazon-sales-channel-home.md) has some common workspace controls including Filters, Default View, Columns, and Export. Not all pages have the same control options.

![Amazon Sales Channel workspace control examples](assets/amazon-workspace-controls.png){width="600" zoomable="yes"}

## Actions

The _[!UICONTROL Actions]_ selector provides a list of actions that are available to a user for a page. When chosen, the action is applied to all selected items. To apply an action to a specific item, select the checkbox in the first column of each item and choose an option under _[!UICONTROL Actions]_.

For example, when the selector is displayed on the _[!UICONTROL Attributes]_ page, it includes the _[!UICONTROL Re-import Product Attribute Values]_ action. Choosing this action pings the corresponding [!DNL Amazon Seller Central] account and refreshes the [!DNL Commerce] data for each of the Amazon store items checked in the left-side column.

![Actions menu example](assets/amazon-sales-channel-home-actions-option.png){width="500"}

## Filters

The _[!UICONTROL Filters]_ control shows options for narrowing the data shown in the table. Filter options are based on the columns selected in the Columns control. Filter options only display for columns enabled in the Columns control.

Filters controls can include dynamic calendars to narrow data for specified dates, drop-down menus for columns that have pre-defined selections, and free-text fields that may contain custom data.

The following example shows the settings for filtering the list of orders to show only orders that meet the following criteria:

- Orders placed between 2/01/2019 and 2/07/2019, and
- Orders with a buyer named of `Smith`, and
- Orders with a status of `Shipped`.

When you have your filtering options set, click **[!UICONTROL Apply Filters]** to filter the data listed. Click Cancel to exit the Filters control without applying.

![Filters control example](assets/workspace-controls-filters.png){width="600" zoomable="yes"}

After you apply filters to your data, **[!UICONTROL Active Filters]** information will appear. You can click the ![Clear filters icon](assets/x-icon-clear-filters.png) icon to clear a specific filter option or click **[!UICONTROL Clear All]** to clear all applied filters.

![Active filters example](assets/applied-filters-line.png){width="700"}

## View

The View control is based on the default columns for page, thus it is named the Default View. You can add or remove available columns using the Columns control. When you customize your columns, you can then save the view as a custom view in the View control.

When you have your columns added or removed from the page display:

1. Click **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**.

1. Enter a name for view.

1. To save the custom view, click the arrow icon.

![View control example](assets/workspace-controls-view.png)

In this example, the _Order Id_ column is added in the Column control and saved as a custom view. Notice that after the custom view name was saved, the name of the View changed from _Default View_ to the entered name.

You can toggle between the views by selecting the desired view in the _[!UICONTROL View]_ menu.

If you want to delete or change the name of your custom view, click the pencil icon. You can then enter a different name, or you can click the trash can icon to delete the custom view. The Default View cannot be deleted.

## Columns

The Columns control allows you to add or remove columns of data from the page display. Each Amazon sales channel page has a preset combination of data columns, but most pages have additional columns available. If no additional columns are available, you can still remove default columns from display.

The following example shows a Columns control. The checked options correspond to the column headers that are shown on the page.

- To add a data column to your page, select the checkbox.
- To remove a data column from your page, do not select the checkbox.

![Columns control example](assets/workspace-controls-columns.png){width="400"}

Checkbox changes display immediately. If you make changes and exit the page, the page returns to the default column display. For changes that you make regularly, you can save the columns changes as a custom view in the View control. Then you can toggle in the View control without having to add or remove columns manually.

You can click **[!UICONTROL Reset]** to set the options back to default settings, or you can click **[!UICONTROL Cancel]** to exit without your changes.

## Export

The Export option allows you to export the data to a data file than can be imported to a third-party software or separate database. Data exported is limited to the data shown. If needed, make sure that you add or remove columns before using the Export control.

When ready to export your data, choose an export format option and click **[!UICONTROL Export]**.

- CSV - a comma-separated value file containing plain text data
- Excel XML - an XML-based, spreadsheet data format (typically used for Excel users)

The generated data file saves automatically to your designated folder for downloads.

![Export control](assets/workspace-controls-export.png){width="250"}
