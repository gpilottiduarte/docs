## Metadata_Start 
## code: en
## title: How to use bulk actions for secrets 
## slug: dsm-bulk-operations 
## seoTitle: Bulk actions for secrets 
## description:  
## contentType: Markdown 
## Metadata_End
You can use bulk operations to enable, disable, or expire the secrets registered in the Segura DevOps Secret Manager (DSM) when necessary.

:::(info) (Info)
As visual feedback, you can follow the stage you are currently at. To do this, look at the top portion of the credentials list screen to see where you are in the bulk operation process.
:::

## Perform bulk operations to DSM secrets

1. On Segura, in the navigation bar, hover over the Products menu and select **DevOps Secret Manager**.
2. In the side menu, select **Secret Management > Secrets**.
3. On the secrets list page, select the secrets you want to change.
4. On the top of the screen will be visible the three operations you can perform: *Enable, Disable or Expire*.

:::(warning) (Caution)
To carry out any of the bulk operations, there must be approvers. For more information, see the documentation on How to register an approver user.
:::

## Bulk Actions for secrets

:::(info) (Info)
The bulk action option allows you to enable, disable or expire several secrets simultaneously. Note, however, that only disabled secrets can be selected for activation.
:::

1. After selecting the secrets, click the option desired on the top of the screen.
2. On the **Bulk operation** screen:
   1. On the **Choose Entities** tab:
      1. Click the **Add** button to open the **Secrets** modal.
      2. On the **Secrets** modal, select the secrets you want do enable.
      3. Click **Add**.
3. Click **Continue**.
4. Click **Save**.

If no errors have occurred, you'll see a success message: "**Bulk operation request created"**. The operation will be executed after approval by those responsible. Together with a shortcut button to the **Bulk operations** section of Segura.

Once the process has been completed, a user who is registered as an approver for the DSM module will need to approve the changes for them to be applied.

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/)