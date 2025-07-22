## Metadata_Start 
## code: en
## title: How to use a DSM automation to inject a secret 
## slug: how-to-use-a-dsm-automation-to-inject-a-secret 
## seoTitle: How to use a DSM automation to inject a secret 
## description:  
## contentType: Markdown 
## Metadata_End

This documento provides information on how to perform a secret injection using Segura DSM automations.

## Requirements

* Have an automation created.

:::(info) (Info)
The execution templates for injecting the secrets can be found in the [Segura repository on GitHub](https://github.com/senhasegura/execution-templates).
:::

## Azure Key Vault

In the **Action** tab, select the **Azure Key Vault - Inject Secret** template to inject and rotate the secrets. After the template execution, access the Azure Portal, search for Key Vault's services, and select the vault where the secret will be injected.

You can analyze the injection details by clicking on Secrets and then clicking on the item created by Segura on the Azure Key Vault.

## Google Secret Manager

In the **Action** tab, select the **Google Secret Manager - Inject Secret** template to inject and rotate secrets. After the template execution, access the **Google Cloud Console** and select the project in the upper selection tab.

You can analyze the details of the injection by selecting on *Google Secret Manager > Security > Secret Management*, and, in this secrets list, click on the item created by Segura.

:::(warning) (Caution)
Note that these two templates aren't registered with Segura by default, so you must add them. You can find the templates in the [Segura repository on GitHub](https://github.com/Segura/execution-templates).
:::

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).