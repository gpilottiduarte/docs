## Metadata_Start 
## code: en
## title: How to manage authorizations per application 
## slug: how-to-manage-authorizations-per-application-in-devops-secret-manager 
## seoTitle: How to manage authorizations per application 
## description:  
## contentType: Markdown 
## Metadata_End

To use Segura's **DevOps Secret Manager (DSM)** features, you must authorize your applications registered with Segura.

## Create an authorization for the application in DevOps Secret Manager

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Application management > Authorization for the application**.
3. On the **Authorization for the application** report, localize the application you want to add an authorization and click the **New authorization** option
4. In the **Add authorization** form:
   1. On the **Security** tab:
      1. **Authorized resources**: indicate which resources the application will be authorized to access.
      2. **Expiration date/time**: in the drop-down menu, select the date from the calendar that opens in the first field, and the time in the second field.
      3. **Status**: indicate if you want the authorization to be active or not.
      4. **Enable encryption of sensitive information**: enables or disables encryption of information marked as sensitive.
      5. **Enable creation of DSM applications?**: enables or disables authorization to create DSM applications.
      6. **Environment**: in the drop-down menu, select the authorization environment.
      7. **System**: in the drop-down menu, select the authorization system.
      8. **Allowed IPs (Put * to allow any IP)**: list of IP addresses that will be allowed. Click on the **Add** button to add as many IPs as you like. To allow any IP address, fill in with `*`.
      9. **Allowed HTTP referrers (empty list for any source)**: list of `HTTP REFERERS` allowed for this authorization. To allow any referer, create an empty list.
      10. **Certificate validation**: enter the certificate's fingerprint that will be used with this authorization.
      11. Click **Continue**.
5. In the **Secrets** tab:
   1. Click the **Add** button to open the **Secrets** modal.
      1. Select the secrets you want to add to the authorization.
      2. Click **Add**.
   2. Click **Continue**.
6. In the **Encryption keys** tab:
   1. Click the **Add** button to open the **Encryption keys** modal.
      1. Select the encryption keys you want to add to the authorization.
      2. Click **Add**.
   2. Click **Continue**.
7. Click **Save** on the **Review** tab.

## Change an authorization for the application in DevOps Secret Manager

To change an authorization per application in the DSM, access the list of applications through **Products menu > DevOps Secret Manager > Applications management > Authorization for the application.**

In the list, identify the application and the authorization you want to change. To do this, follow the steps below:

1. Click the **Actions** button and select **Edit**.
2. In the **Application Authorization** form, make the necessary changes.
3. Click **Save** on the **Review** tab.

## How to view an authorization

To view an authorization by application in the DSM, access the list of applications through **Products Menu > DevOps Secret Manager > Applications management > Authorization for the application.**

In the list, identify the application and authorization you want to view. To do this, follow the steps below:

1. Click the **Actions** button and select the **View authorizations** option.
2. In the **Application authorizations** you can check the following information about the authorizations:
   1. **Authentication method**: authentication method used by the application.
   2. **Application**: name of the application.
   4. **Client ID**: client identification. It must be a string as this example: `5e1983dc7014e5caab711aa73cd714400622256655d`.
   5. **Client secret**: secret of the client. Must be a string as this example: `9753d43831513ebf60c5f02dc7505f42`.

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).