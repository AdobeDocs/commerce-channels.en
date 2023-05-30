---
title: Cancel an unshipped Amazon order
description: Cancel a pending or partially shipped (unshipped) order through your Amazon [!DNL Seller Central] account.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
---
# Cancel an unshipped Amazon order

Amazon orders can only be canceled if they are in an `Unshipped` status. If the order is pending or partially shipped (unshipped), the order can only be canceled through your [!DNL Amazon Seller Central] account. If the item has been shipped, returns and exchanges must also be handled in your [!DNL Amazon Seller Central] Account.

>[!NOTE]
>
>For tasks other than cancelling an order:
>
>- If you have [order import](./order-settings.md) enabled, orders are managed in the [[!DNL Commerce] orders workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).
>- If [order import](./order-settings.md) is disabled, you must manage your orders in [!DNL Amazon Seller Central].

## Cancel an order in `Unshipped` status

1. Click **[!UICONTROL View Store]** on the store card.

1. In the _[!UICONTROL Recent Orders]_ section of the store dashboard, click an order number.

    The _[!UICONTROL Amazon Order Details]_ page appears.

1. Click **[!UICONTROL Cancel Order]** in the header bar.

   This option only appears for orders in `Unshipped` status.

1. For **[!UICONTROL Reason for cancellation]**, choose an option.

1. Click **[!UICONTROL Confirm]**.

    The order is canceled, and the status is updated to `Canceled` in the order details.

The cancellation notification is sent to your [!DNL Amazon Seller Central] account, and the customer associated with the order is also notified. The status of the corresponding [!DNL Commerce] order, if any, changes to `Complete`.
