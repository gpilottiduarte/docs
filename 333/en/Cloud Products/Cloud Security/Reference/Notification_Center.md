# Notification Center

This document contains detailed information about the **Notification Center**.

The **Notification Center** is a **Cloud Security** feature designed to keep you informed about all relevant activity related to your products, such as software updates and specific alerts.

## Path to access

1. On **Cloud Security**, in the top bar, click the **Notification Center** icon, represented by the bell.

A sidebar will open with all your notifications.

## Notification center sidebar

The following table shows all fields and buttons on the Notification center sidebar:

| Item | Type | Description |
| :---- | :---- | :---- |
| **Refresh** | **Button.** | Refresh all notifications. |
| **Mark all as read** | **Button.** | Marks all notifications as read. |
| **Slack integration** | **Button.** | Integrate the notification center with Slack. See [How to integrate the Notification Center with Slack](/v3-33/docs/how-to-integrate-the-notification-center-with-slack) for more information. |
| **Date** | **Text.** | Date when the notification was sent. Date format is: ```DD-MM-YYYY hh:mm:ss```. |
| **Product** | **Text.** | Name of the product that sent the notification. |
| **Tenant** | **Text.** | The tenant from which the notification comes. You can receive notifications from a tenant even if you aren't logged in to it. |
| **Show more** | **Button.** | Show more notifications. |

## Types of notifications

The following table shows all types of notifications available:

| Notification | Description | User that receives the notification |
| :---- | :---- | :---- |
| **Account Discovery Finished** | First synchronization or resynchronization finished successfully. | User that did the synchronization or resynchronization. |
| **Account Discovery Finished With Error** | First synchronization or resynchronization finished with an error. | User that did the synchronization or resynchronization. |
| **Account Security Policies Updated** | Security policies changed. | Auditors, and tenant administrators. |
| **Account Security Policies Disabled** | Security policies changed to the global default. | Auditors, and tenant administrators. |
| **AWS Account Invalid Key** | Invalid AWS account key. | Tenant administrators. |
| **Azure Account Invalid Key** | Invalid Azure account key. | Tenant administrators. |
| **Google Cloud Account Invalid Key** | Invalid Google Cloud account key. | Tenant administrators. |

## Slack

The following table shows all fields and buttons on the **Slack** screen:

| Item | Type | Description |
| :---- | :---- | :---- |
| **Add** | **Button.** | Add a new Slack webhook. |
| **Channel name** | **Text field.** | Enter the channel name. |
| **URL** | **Text field.** | Add the webhook URL. |
| **Notification type** | **Dropdown menu.** | Select the types of notifications to receive on Slack. |
| **What can I do here?** | **Button.** | Redirect the user to the documentation related to this screen. |
| **Activated** | **Toggle button.** | Activate or deactivate the integration.  |
| **Edit** | **Button.** | Edit the integration. |