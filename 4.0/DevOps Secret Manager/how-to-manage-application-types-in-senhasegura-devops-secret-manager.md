## Metadata_Start 
## code: en
## title: How to manage application types 
## slug: how-to-manage-application-types-in-senhasegura-devops-secret-manager 
## seoTitle: How to manage application types 
## description:  
## contentType: Markdown 
## Metadata_End

## Register an application type

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Application management > Application types**.
3. Click the **Add** button.
4. In the **Add application type** screen, fill in the information:
    1. **Name**: enter a name for your application type.
    2. **Status**: select if you want your application type to be created as enabled.
    3. **Description**: enter a description for the registered application type. This description will be useful for understanding what the registered application type is about.
5. Click **Save.**

## Change an application type

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Application management > Application types**.
3. On the **Application types** report, click the **Actions** button and select **Edit**.
4. The **Application Type** form will open in edit mode, modify the information according to your needs.
5. Click **Save**.

## Inactivate an application type

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Application management > Application types**.
3. On the **Application types** report, click the **Actions** button and select **Edit**.
4. The **Application Type** form will open in edit mode, modify the **Status** field by unselecting it.

:::(info) (Info)
When inactivated, the application type becomes unavailable in all applications and will no longer appear in the applications that were previously registered with it.
Note that inactivating an application type can affect the settings of access groups. For example, depending on the configuration made, users can lose/gain access privileges.
:::

## Reactivate an application type

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Application management > Application types**.
3. On the **Application types** report, click the **Actions** button and select **Edit**.
4. The **Application Type** form will open in edit mode, modify the **Status** field by reselecting it.

:::(warning) (Important)
The reactivated application type won't be added back to the applications to which it was previously linked. So, if you inactivate an application type, it will lose its relationship with the application, and when you reactivate it, this relationship won't be re-established automatically.
:::

***

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).