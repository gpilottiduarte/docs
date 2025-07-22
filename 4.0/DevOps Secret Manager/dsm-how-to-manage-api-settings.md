## Metadata_Start 
## code: en
## title: How to manage API settings 
## slug: dsm-how-to-manage-api-settings 
## seoTitle: How to manage API settings 
## description:  
## contentType: Markdown 
## Metadata_End
You can manage **DevOps Secret Manager** via its API. To use the **DSM API**, you need to authorize the credentials you want to use. To do so, follow the steps below:

1. On Segura, in the navigation bar, hover over the **Products menu** and select **DevOps Secret Manager**.
2. In the side menu, select **Access Control > API Settings.**
3. The report that will be opened will contain all the credentials and applications with access to the DSM API.
4. On the **Credentials** tab
   1. **A2A Application**:
      1. Click the **Add** button to open the **A2A Applications** modal.
      2. Select the applications you want to add. You can select more than one.
      3. Click the **Add** button.
   2. **Credentials**:
      1. Click on the **Add** button to open the **Credentials** modal..
      2. In the **Credentials** modal, select the credentials you want access to the DSM API.
      3. Click the **Add** button.
         - PAM credentials created from **A2A applications** defined in the **A2A Application** field will be released for management in the DSM APIs.
         - Credentials defined in the **Credentials** field will be released for management in the DSM APIs.
   3. Click **Continue**.
5. on the **Cloud credentials** tab:
   1. Click the **Add** button to open the **User/Service Account** modal.
   2. Select the user/service accounts you want to add to the DSM API.
   3. Click **Continue**.
      - Cloud credentials that belong to the users defined in the **User/Service Account** field will be available for management in the DSM APIs.
3. Click **Save** on the **Review** tab.

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).