## Metadata_Start 
## code: en
## title: How to integrate DSM with Kubernetes 
## slug: how-to-integrate-dsm-with-kubernetes 
## seoTitle: How to integrate DSM with Kubernetes 
## description:  
## contentType: Markdown 
## Metadata_End
## Requirements:

1. You should have Kubernetes properly installed.
2. You should have the `kubectl` tool installed.
    - Follow the installation steps provided in the [Getting started - External Secrets Operator](https://external-secrets.io/latest/introduction/getting-started/) documentation.

## Configuration in the Segura

[colocar os links para todos esses guias]

1. Create an **Access policy** in the DSM.
2. Create a **Secret** in Segura.
3. Create an **Application** in Segura.
4. Create an **Authorization** for the newly created application.
5. Add the **Secret** to the **Authorization of the application**.
6. Copy the values of the **Client ID** and **Client Secret** fields from the application's authorization.
7. Create a file with the `.yml` extension in Kubernetes.
8. Fill in the `.yml` file with the **Client ID** and **Client Secret** values you copied earlier.
9. Execute the following command: `kubectl apply -f nomedoarquivo.ymlc`

In Kubernetes, follow the steps in the Segura documentation on External Secrets, available at [Segura DevOps Secrets Management (DSM)](https://external-secrets.io/latest/provider/senhasegura-dsm/).

By following these steps, the integration between DSM and Kubernetes via External Secrets will be configured, guaranteeing secure and effective management of the sensitive information needed to operate your environment

## Validate the integration

| Command | Description |
| --- | --- |
| `kubectl get externalsecret -o wide` | Check the synchronization status. |
| `kubectl describe externalsecret example-secret` | Check the synchronization status. |
| `kubectl get pods -A` | Check the Pod creation. |
| `kubectl get secrets/example-secret -n namespace -o yaml` | Check the External Secrets contents. |
| `kubectl get secrets/example-secret -o yaml` | Check if the synchronized secret has been created and that the data has been retrieved. |
| `kubectl logs -f pod/external-secrets-<CHANGEME> -n external-secrets` | Check the External Secrets logs. |

---

Do you still have questions? Reach out to the [Segura Community](https://community.senhasegura.io/).