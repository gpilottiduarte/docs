## Metadata_Start 
## code: en
## title: How to manage access policies 
## slug: dsm-how-to-manage-access-policies 
## seoTitle: How to manage access policies 
## description:  
## contentType: Markdown 
## Metadata_End
## Create an access policy

:::(info) (Info)
Synchronized users will have their permissions replaced if synchronization is enabled. Check your synchronization policies for changes.
:::

To create an access policy in DevOps Secret Manager, follow the instructions below:

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager.**
2. In the side menu, select **Access control > Access policies.**
3. You'll be taken to the page with a list of all the policies registered with Segura.
4. Click the **Add** button.

In the **Add access policy** form, fill in the following fields:
1. On the **General** tab:
   1. **Access policy name**: fill in a name for the access policy. This is the name that will identify the access policy in Segura.
   2. **Status**: check to enable the new policy.
   3. **Description**: enter a brief description of the access policy.
   4. Click **Continue**.
2. On the **Users** tab:
   1. Click the **Add** button to open the **Users** modal.
   2. On the **Users** modal, select the user you want to add to the new policy.
   3. Click **Add**.
   4. Click **Continue**.
3. On the **Secrets** tab:
   1. **Users can view secret**: check to allow users to view the secrets registered in Segura.
   2. **Require reason**: check to require the user to justify viewing a registered secret.
   3. **Require approval**: check to require that viewing the secret requires approval. This approval must be done by a user with the role of approving user.
   4. **Approvals required:** enter the number of approvals required for the user to view the secret. By default, the value is 1.
   5. **Disapprovals required to cancel:** enter the number of approvals required to cancel the user's request. By default, the value is 1.
   6. **Approval in levels**: check to indicate if you want the user to require approvals at different levels.
   7. **Governance ID required when justifying?:** check if you want the user to need a governance code filled in on the justification request. By default, this is set to No.
  8. Click **Continue**.
4. On the **Approvers** tab:
   1. Click the **Add** button to open the **Approvers** modal.
   2. On the **Approvers** modal, select the user you want to add to the new policy.
   3. Click **Add**.
   4. **Governance ID required when justifying**: indicates if every change will ask for a governance ID.
   5. **Always add user manager do approvers**: indicates if the user's manager will always be part of the approvers policy of this user.
   6. Click **Continue**.
5. On the **Filters** tab:
   1. In the **Application** section, fill in the following information:
      1. **Application names (comma-separated)**: indicate which applications this access policy will be allowed to use. Names must be separated by a comma.
      2. **Application tags (comma-separated)**: indicate which application tags this access policy will be allowed to use. The tags must be separated by a comma.
      3. **Line of business**: check the lines of business to which the indicated applications belong.
      4. **Application Types**: checkbox with the types of applications to which the indicated applications belong.
         - **Be aware of the following behavior of access policies**: by setting the filtering options to `Empty` in **Line of Business** and **Application Types**, users who are members of the access policy will only see applications with no data in these fields. Thus, selecting the `Empty` option will result in the display of applications with unfilled **Line of Business** and **Application Types** fields. On the other hand, if the `Empty` option isn't selected, applications with these empty fields won't appear in the results.
         - You can use the `[#username#]` wildcard, which will be replaced by the user's name during access processing.
   2. In the **Authorizations** section, fill in the following information.
      1. **Systems (comma-separated)**: indicate the systems this access policy will be allowed to access. System names must be separated by a comma.
      2. **Environments (comma-separated)**: indicate the environments this access policy will be allowed to access. The names of the environments must be separated by commas.
         - Access will only be granted to authorizations belonging to applications granted by the application rules of this access policy.
   3. Click **Continue**.
6. On the **Criteria** tab:
   1. **Secrets names (comma-separated)**: indicate the secrets the access policy will be allowed. The secrets must be separated by a comma.
   2. **Secret environments (comma-separated)**: indicate the environments the secrets will be allowed to access. The names of the secret environments must be separated by a comma.
   3. **Secret tags (comma-separated)**: indicate which secret tags this access policy will be allowed to use. The tags must be separated by a comma.
      - Note that access will only be granted to secrets who:
         - Don't belong to any authorization.
         - Belongs to an authorization granted by the authorization rules of this access policy.
   4. Click **Continue**.
7. To finish creating the access policy, click **Save** on the **Review** tab.

## Update an access policy

To update an access policy already registered with Segura, follow the steps below:

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Access control > Access policies**.
3. You'll be taken to the page with a list of all the policies registered with Segura.
4. Identify the access policy you want to update and click **Edit**.

You'll be directed to the **Edit access policy** screen with the same tabs and fields of the **Add access policy** screen. Edit the information you want and save it.

## Synchronize access policies

Occasionally, policy information may not be visible to users, or can be displayed incorrectly due to configuration problems. The **Synchronize policies** feature can synchronize all policy information in such cases. Therefore, if any information isn't visible to you, it may be due to some initial processing problem, which can be corrected by reprocessing.

To use this feature, follow the steps below:

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager.**
2. In the side menu, select **Access control > Access policies.**
3. On the **Access policies** screen, click the **Synchronize** buton.
4. In the confirmation modal, click **Yes**.

:::(error) (Attention)
When reprocessing policies, some users may lose access to DSM entities.
:::

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).