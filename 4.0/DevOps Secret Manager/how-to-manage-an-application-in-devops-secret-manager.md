## Metadata_Start 
## code: en
## title: How to manage an application 
## slug: how-to-manage-an-application-in-devops-secret-manager 
## seoTitle: How to manage an applications 
## description:  
## contentType: Markdown 
## Metadata_End

## Requirements
* Have registered applications to allow them to access the DSM's secrets.

## Register an application with DevOps Secret Manager

To register a new application, follow the steps below:

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Application management > Applications**.
3. Click the **Add** button.
4. On the **Add application** form:
   1. On the **Settings** tab:
      1. **Application name**: enter a name to identify the application.
      2. **Authentication method**: in the drop-down menu, select the desired method.
      3. **Line of business**: in the drop-down menu, select the line of business for that application. You can register new lines of business within Segura.
      4. **Application type**: in the drop-down menu, select the type of application being registered. You can register new application types within the Segura instance.
      5. **Status**: check to enable or disable the application.
      6. **Tags**: enter the tags you want to link with the application. They must be separated by commas.
      7. **Description**: enter the description text for the application.
      8. **Amazon AWS ARNs**: click the **Add** button to add a new entry on the table. In this new entry, fill in the Amazon AWS ARN of the resource that will be registered with the application.
      9. Click **Continue**.
5. On the **Automatic provisioning** tab: 
   1. **Automatic provisioning of secrets**: check to open the options to the automatic provision of secrets.
   2. **Cloud dynamic provisioning profile**: click the **Add** button to add a new entry on the table.
      1. On the table, select profile you want to use from the dropdown menu.
   3. **Credential dynamic provisioning profile**: click the **Add** button to add a new entry on the table.
      1. On the table, select the **Device** and the **Provisioning profile** you want to use from the dropdown menus.
   4. Click **Continue**.
6. Click **Save** on the **Review** tab.

:::(info) (Info)
AWS ARN refers to the unique identifiers of AWS resources.
:::

## Change an application registered in DevOps Secret Manager

To change an application already registered in the DSM, access the list of applications through **Products menu > DevOps Secret Manager > Application management > Applications.**

In the list, identify the application you want to change. To do this, follow the steps below:

1. Click the **Actions** button and select the **Edit** option.
2. In the **Application Configuration** form, make the necessary changes and save it.

## View an application registered in DevOps secret Manager

To view an application already registered in the DSM, access the list of applications through **Grid Menu > DevOps Secret Manager > Applications > Applications**.

In the list, identify the application you want to view. To do this, follow the steps below:

1. Click the **Actions** button and select the **View** option.
2. The **Application Configuration** screen will open in view mode.

In this window, you can view the information about the application:

1. **Authentication method**: authentication method registered with the application.
2. **Application**: name of the application.
3. **Client ID**: client identification. It must be a string in this pattern: `5e1983dc2023e5caab985aa73cd7144006221333d`.
4. **Client Secret**: client secret. To view it, click the eye icon.
5. **System**: client's system.
6. **Environment**: application environment.

## View an authorization by application

To view the authorizations of an application already registered in the DSM, access the list of applications through **Grid Menu > DevOps Secret Manager > Applications > Applications.**

In the list, identify the application you want to view. To do this, follow the steps below:

1. Click the **Actions** button and select the **Authorizations** option.
2. In the **Authorizations for the application** screen, you can analyze a list of all the authorizations that this application has.

## Manage the automatic provisioning of secrets

When you register a new application, you can determine whether it will automatically provision the secrets stored in the DSM.

## Requirements

* Registered provisioning profiles.

To manage the automatic provisioning of secrets, follow the steps below:

1. In the **Application Configuration** screen: 
   1. In the **Automatic Provisioning** tab: 
      1. Check the **Automatic provisioning of secrets** toggle.
      2. **Dynamic Provisioning** section:
         1. **Cloud dynamic provisioning** **profile**.
            1. Click the **Add** button to add a new entry on the table.
               1. In the drop-down menu, select one of the profiles you created earlier.
      3. **Credential dynamic provisioning** **profile**.
         1. Click the **Add** button to add a new entry on the table and fill in the fields:
            1. **Devices**: in the drop-down menu, select the credential's device.
            2. **Provisioning profile**: in the drop-down menu, select the profile you created earlier.
   3. Click **Continue**.
2. Click **Save** on the **Review** tab.

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).