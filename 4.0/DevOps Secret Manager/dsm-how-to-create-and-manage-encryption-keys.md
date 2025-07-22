## Metadata_Start 
## code: en
## title: How to create and manage encryption keys 
## slug: dsm-how-to-create-and-manage-encryption-keys 
## seoTitle: Como criar e gerenciar chaves de criptografia 
## description:  
## contentType: Markdown 
## Metadata_End
This tutorial is a step-by-step guide on creating and managing encryption keys in the **DevOps Secret Manager** of Segura.

## Requirements
- You must have the necessary permissions in the role to which it is associated.

## Add an Encryption key

1. On Segura, in the navigation bar, hover over the Products menu and select **DevOps Secret Manager**.
2. On the side menu, select **Encryption > Encryption keys**.
3. Click the **Add** button.
4. On the **Ass encryption key** screen, fill in the following fields:
    - **Name***: name of the cryptographic key.
    - **Encryption algorithm***: choose the encryption algorithm.
    - **Expiration date**: key expiration date and time.
    - **Active**: check to enable the key.
    - **Description**: description associated with the key.
6. Click **Save**.

## View Encryption key details

1. On the **Encryption key** report, click the **Action** button and select **Details**.
2. In the open pop-up window, you can view the fields **Name**, **Version**, **Encryption** **algorithm**, **Expiration date**, **Active**, and **Description**.

:::(Info) (Info)
  With each key update, the version field will also be updated; the version statement can be accessed through the button **Show versions** inside the three vertical dots icon in the column Action.
:::

## How to Encrypt data

1. On the **Encryption key** report, click the **Action** button and select **Operate**.
2. Select the **Encryption** tab.
3. Type the data you want to encrypt on the **Value to encrypt** field.
3. Click the **Encrypt** button.
4. The field **Encrypted value** will display the encrypted value for your data.

In the menu **Events > Audit Tracking**, it’s possible to check the logs for each encryption attempt.

## How to decrypt data

:::(Info) (Info)
The key must contain the same encryption algorithm for decryption to be performed.
:::

1. On the **Encryption key** report, click the **Action** button and select **Operate**.
2. Select the **Decrypt** tab.
3. Type the data you want to encrypt on the **Value to decrypt** field.
3. Click the **Decrypt** button.
4. The field **Decrypted value** will display the encrypted value.