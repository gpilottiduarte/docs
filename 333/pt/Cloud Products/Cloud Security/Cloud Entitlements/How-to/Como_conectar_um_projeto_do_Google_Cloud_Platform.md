# Como conectar um projeto do Google Cloud Platform

Neste artigo, você aprenderá como conectar **Cloud Entitlements** aos seus projetos do Google Cloud Platform (GCP).

## Requisitos

- Uma **Conta de serviço** com as seguintes funções:
    - `iam.serviceAccountKeys.list`
    - `iam.serviceAccounts.list`
    - `iam.roles.list`
    - `iam.roles.get`
    - `resourcemanager.organizations.getIamPolicy`
    - `resourcemanager.projects.getIamPolicy`
    - `resourcemanager.projects.list`
- Uma **Chave de acesso** associada à Conta de serviço.
- As seguintes APIs do GCP ativas:
    - Resource Manager.
    - Identity and Access Management (IAM).
    - Cloud Assets.

---

## Conectar um projeto do Google Cloud Platform

Para conectar seu projeto GCP ao **Cloud Entitlements**, siga estas etapas:

1. Vá para o menu à esquerda de **Cloud Entitlements**.
2. Clique em **Configuração** para abrir o menu suspenso.
3. Selecione **Google Cloud Platform**.
4. No canto superior direito, clique em **+ Conectar**.
5. Insira um **Nome** para identificar seu projeto dentro do **Cloud Entitlements**.
6. Insira a **ID do Projeto**.
7. Se necessário, atribua etiquetas para o projeto. Separe cada etiqueta usando a tecla **Enter**.
8. Faça o upload do **arquivo JSON** da chave da conta de serviço do seu projeto GCP.
9. Clique em **Salvar**.

Se a conexão for bem-sucedida, seu projeto GCP aparecerá na lista de projetos conectados.

::: (Error) (Importante)
Se a conexão não for bem-sucedida, confira a ID do projeto, as funções atribuídas e se as APIs necessárias foram ativadas. Você não pode usar um ID de um projeto que já está conectado ao **Cloud Entitlements**.
:::

Para fazer quaisquer alterações necessárias, clique no botão **Ações**, representado por três pontos verticais, e clique em **Editar**.

Além disso, você pode ativar ou desativar o projeto, ligando ou desligando o **Status switch**.