# How to connect a Google Cloud Platform project

In this article, you'll learn how to connect **Cloud Entitlements** to your Google Cloud Platform (GCP) projects.

## Requirements

- A **Service account** that contains the following roles:
  - `iam.serviceAccountKeys.list`
  - `iam.serviceAccounts.list`
  - `iam.roles.list`
  - `iam.roles.get`
  - `resourcemanager.organizations.getIamPolicy`
  - `resourcemanager.projects.getIamPolicy`
  - `resourcemanager.projects.list`
- A **Key** provisioned for the Service account.
- The following GCP APIs enabled:
  - Resource Manager.
  - Identity and Access Management (IAM).
  - Cloud Assets.

---

## Connect a Google Cloud Platform project

To connect your GCP project to **Cloud Entitlements**, follow these steps:

1. Go to **Cloud Entitlements** left menu.
2. Click **Cloud setup** to open a dropdown menu.
3. Select **Google Cloud Platform**.
4. On the upper-right corner, click **+ Connect**.
5. Select the option **Project**.
6. Enter a **Name** to identify your GCP project within **Cloud Entitlements**.
7. Enter your **Project ID**.
8. Upload the Service account key's **JSON file**.
9. If needed, attribute tags to the project. Separate each tag by pressing the **Enter** key.
10. Click **Save**.

If connected successfully, your GCP project will appear in the list of connected projects.

<!-- Fix callout -->
:::(Error) (Important)
If the connection is unsuccessful, review the project ID, the roles, and the enabled APIs. You can't use an ID from a project that is already connected to **Cloud Entitlements**.
:::

To make any necessary changes, click the **Actions** button, represented by three vertical dots, and click **Edit**.

Additionally, you can activate or deactivate the project by turning the **Status switch** on or off.
