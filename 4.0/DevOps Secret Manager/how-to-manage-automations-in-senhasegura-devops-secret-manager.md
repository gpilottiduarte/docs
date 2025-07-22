## Metadata_Start 
## code: en
## title: How to manage DSM automations 
## slug: how-to-manage-automations-in-senhasegura-devops-secret-manager 
## seoTitle: How to manage DSM automations 
## description:  
## contentType: Markdown 
## Metadata_End
Within Segura **DevOps Secret Manager (DSM)**, you can register automations to simplify everyday actions.

## Requirements

* A previously created application or secret.
* A credential that will be used to perform the automation action.
* A device on which the automation will be executed.
* An execution template of the **Secret Management Automation** type for the desired executor.

## Add an automation to DSM

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager.**
2. In the side menu, select **Automations > Automations**.
3. Click the **Add** button.
4. In the **Add automation** form:
   1. In the **Information** tab:
      1. **Name**: name that identifies the automation within the Segura instance.
      2. **Status**: check to choose if the automation will be registered as active.
      3. **Description**: fill in a description of the automation.
      4. **Tags**: add the tags that will identify the automation.
      5. Click **Continue**.
   2. In the **Trigger** tab:
      1. In **When this happens ...** section, you'll define the trigger that will start the automation. To do this, fill in the following fields:
         1. Click the **Add** button to open the **Triggers** modal.
         2. In the **Triggers** modal, select the triggers (actions) that will be used to start the automation. You can choose as many as you like.
         3. Click **Add**.
      2. In **... In this Application or Secrets ...** section, you'll define which applications or secrets will be affected by the trigger. To do this, fill in the following fields:
         1. **Applications**:
            1. Click the **Add** button to open the **Applications** modal.
            2. In the **Applications** modal, select the applications affected when the trigger is started. You can choose as many as you like.
            3. Click **Add**.
         2. **Secret**:
            1. Click the **Add** button to open the **Secrets** modal.
            2. In the **Secrets** modal, select the secrets that will be affected when the trigger is started. You can choose as many as you like.
            3. Click **Add**.
         3. Click **Continue**.
   3. In the **Action** tab:
      1. In **Execute this template …** section, you'll define the template containing the commands executed in the application(s) or secret(s) when the trigger is activated. To do this, fill in the following fields:
         1. From the **Change plugin** drop-down menu, select one of the plugins that are registered with Segura.
         2. From the **Change template** drop-down menu, select one of the templates for that plugin.
            1. When creating automation, you can create a new template by clicking the **Create template** button.
               - When a template is created using this creation option, the template won't automatically appear in the drop-down menu list. You'll need to re-enter all the information by reloading the page or manually adding a new automation.
      2. In **... in this devices …** section, you'll add the devices on which the template will run. To do this, fill in the following fields:
         1. Click the **Add** button to add a new entry to the table.
            2. From the **Device** drop-down menu, select one of the devices registered with Segura.
            3. From the **Credential** drop-down menu, select the credential used for authentication on the indicated device.
      3. Click **Continue**.
5. Click **Save** on the **Review** tab.

## Edit an automation in DSM

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager.**
2. In the side menu, select **Automations > Automations**.
3. Localize the automation you want to edit, click the **Actions** button and then select **Edit**.
5. The **Automation** form will open in edit mode.
6. Change what you want and click **Save** on the **Review** tab.

::: (info) (Info)
You'll find an eye icon in the upper-right corner of the **Automation** form. You can access information about the automation by hovering your mouse over it. This information includes the name and username of the person who created the automation and the name and username of the last person who made changes to it.
:::

## View the details of automation in DSM

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager.**
2. In the side menu, select **Automations > Automations**.
3. Localize the automation you want to edit, click the **Actions** button and then select **Details**.
4. The **Automation** screen will open with the following information:
   1. **ID**: contains the code of the automation.
   2. **Name**: contains the name of the automation.
   3. **Creation date**: the date when the automation was created.
   4. **Last execution:** the date when the automation was last run.
   5. **Status**: indicates the current status of the automation.
   6. **Description**: a brief description of the automation.
   7. **Tags**: the tags that help categorize the automation.
   8. **Triggers**: the actions that will activate the templates.
   9. **Applications**: the applications that will be affected by the template.
   10. **Secrets**: the secrets that will be affected by the template.
   11. **Plugin**: the plugin that is used in automation.
   12. **Template**: the name of the template that will perform the action when the trigger is activated.
   13. **Device (credential)**: contains the address of the device and the credential that will be used for authentication.

## Disable an automation in DSM

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager.**
2. In the side menu, select **Automations > Automations**.
3. Localize the automation you want to edit, click the **Actions** button and then select **Disable**.
4. A modal will display a message that the automation was successfully disabled.

:::(warning) (Warning)
Disable an automation has no intermediate steps, so when you click Delete, the automation will be disabled without any extra confirmation.
:::

## Activate automation in DSM

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager.**
2. In the side menu, select **Automations > Automations**.
3. ON the filters, select the **Disable** option from the **Status** drop-down menu and click **Filter**.
4. In the list, identify the automation you want to activate, click the **Actions** button and then select the **Edit** option.
5. The **Automation** window will open in edit mode.
6. In the **Status** field, check the toggle do enable.
7. Click **Save** on the **Review** tab.

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).