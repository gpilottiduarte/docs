## Metadata_Start 
## code: en
## title: How to manage dynamic provisioning in DSM 
## slug: how-to-manage-dynamic-provisioning-in-dsm 
## seoTitle: How to manage dynamic provisioning in DSM 
## description:  
## contentType: Markdown 
## Metadata_End

This document provides a guide to use the Dynamic Credentials feature on Segura DSM.

## Important
To use the dynamic credentials, you must first register a profile.

## Requirements

* Have an application registered with Segura DSM.
* Have at least one secret registered in Segura DSM.
* Have at least one credential registered with Segura.
* Have at least one device registered with Segura.

## Create dynamic provisioning profile

1. On Segura, in the navigation bar, hover over the Products menu and select **PAM Core.**
2. In the side menu, select **Management > Dynamic credentials > Profiles**.
3. Click the Add button.
4. On the **Credential provisioning profile**:
   1. **Identifier**: enter an identifier for your dynamic provisioning profile within Segura.
   2. **Status**: select the Yes radio box to create an active profile. If you want to create an inactive profile, select the No option.
   3. **Type**: select the type of profile from the drop-down menu.
   4. In the **Credential to execute** section:
      1. **Use a registered credential to access all devices:** select this checkbox if you want to use a PAM Core credential to access the devices.
      2. **Access credential registered in the system:** if you select the above option, the drop-down menu will become accessible, and you can choose one of the credentials already registered in Segura.
      3. **Credential username:** if you don't want to use a registered credential, enter the username in this field to access the devices.
   5. In the **Templates** section:
      1. **Credential creation template:** select the template that will be used to create the dynamic provisioning credential from the drop-down menu.
         - The plus icon next to the drop-down menu allows you to create another creation template and load it.
      2. **Credential removal template:** select the template that will be used to remove the dynamic provisioning credential from the drop-down menu.
         - The plus icon next to the drop-down menu allows you to create another removal template and load it.
   6. **Roles**: add the roles you want the dynamic provisioning credential to assume. A comma must separate the roles.
      - By hover over the question mark icon, a help modal will open to explain the roles.
   7. In the field below the **Template** section, you can define a TTL (*Time To Live*) interval, in seconds, for the dynamic credential. The default is `3600` seconds.
8. Click **Confirm**.

## Edit a dynamic credential profile

1. On Segura, in the navigation bar, hover over the Products menu and select **PAM Core.**
2. In the side menu, select **Management > Dynamic credentials > Profiles**.
3. In the list of profiles, identify the profile you want to change, click the **Actions** button and select the **Edit** option.
4. The **Credential provisioning profile** form will open in edit mode.
5. Make the necessary changes and click **Confirm**.

:::(info) (Info)
By hovering over the icon represented by the eye at the upper-right corner of the creation profile form, you can analyze some information, such as the date and time of creation and the date and time of updating that credential. Note: the eye icon is only displayed when editing the dynamic provisioning credential.
:::

## Activate automatic renewal

Configuring an application with dynamic provisioning profiles allows the automatic rotation of secrets at predetermined intervals, creating and registering new credentials without interrupting the use of old ones until they are updated through the rotation process.

To enable the automatic renewal of a secret, follow the steps below:

1. On Segura, in the navigation bar, hover over the Products menu and select **DevOps Secret Manager**.
2. In the side menu, select **Secret management > Secrets**.
3. Update or create a new secret.
4. In the **Secret Configuration** form, on the **Auto renew** tab, enable the options:
   1. **Cloud credentials:** check and enter a time interval in the **Minutes between each renewal** option.
   2. **Ephemeral credentials**: check and enter a time interval in the **Minutes between each renewal** option.
   3. **Credentials:** check and enter a time interval in the **Minutes between each renewal** option.
5. Click **Save** on the **Review** tab.

:::(info) (Info)
For all options, the minimum time interval is 10 minutes.
:::

### Important

Enabling automatic credential renewal will trigger a periodic password change on a secret's credentials, which can cause systems to stop,depending on how they are using the credentials. Therefore, always make sure that the application also receives this update.

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).