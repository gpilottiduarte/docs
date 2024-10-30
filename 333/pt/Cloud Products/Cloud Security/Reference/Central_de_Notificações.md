# Central de Notificações

Este documento contém informações detalhadas sobre a **Central de Notificações.**

A **Central de Notificações** é uma funcionalidade do **Cloud Security**, desenvolvida para manter o usuário informado sobre todas as atividades relevantes relacionadas aos seus produtos, como atualizações de software, e alertas específicos.

## Caminho para acesso

1. No **Cloud Security**, na barra superior, clique em **Central de Notificações**, representada pelo ícone de sino.

Uma barra lateral será aberta com todas as suas notificações.

## Barra lateral

A tabela a seguir exibe todos e campos presentes na barra lateral **Central de Notificações**:

| Item | Tipo | Descrição |
| :---- | :---- | :---- |
| **Atualizar** | **Botão.** | Atualiza todas as notificações |
| **Marcar tudo como lido** | **Botão.** | Marca todas as notificações como lidas. |
| **Integração com Slack** | **Botão.** | Realiza a integração entre a **Central de Notificações** e o **Slack**. Veja [Como integrar a Central de Notificações com o Slack](/v3-33/docs/pt/how-to-integrate-the-notification-center-with-slack) para mais informações. |
| **Data** | **Texto.** | Data de quando a notificação foi enviada. O formato da data é: ```DD-MM-YYYY hh:mm:ss```. |
| **Produto** | **Texto.** | Nome do produto que enviou a notificação. |
| **Tenant** | **Texto.** | Tenant de onde vem a notificação. Você recebe notificações de um tenant mesmo se não estiver logado nele. |
| **Mostrar mais** | **Botão.** | Mostra mais notificações. |

## Tipos de notificações

A tabela a seguir exibe todos os tipos de notificações disponíveis:

| Notificações | Descrição | Usuário que recebe as notificações |
| :---- | :---- | :---- |
| **Descoberta Finalizada** | Primeira sincronização ou ressincronização de conta concluída com sucesso. | Usuário que fez a sincronização ou ressincronização. |
| **Descoberta Finalizada Com Erro** | Primeira sincronização ou ressincronização de conta concluída com erro. | Usuário que fez a sincronização ou ressincronização. |
| **Políticas de Segurança Atualizadas** | Políticas de segurança da conta alteradas. | Auditores e administradores de *tenants*. |
| **Políticas de Segurança Desabilitadas** | Políticas de segurança alteradas para o padrão global. | Auditores e administradores de *tenants*. |
| **Chave Inválida da Conta AWS** | Chave da conta AWS inválida. | Administradores de *tenants*. |
| **Chave Inválida da Conta Azure** | Chave da conta Azure inválida. | Administradores de *tenants*. |
| **Chave Inválida da Conta Google Cloud** | Chave da conta Google Cloud inválida. | Administradores de *tenants*. |

## Slack

A tabela a seguir exibe todos os campos e botões na tela **Slack**:

| Item | Tipo | Descrição |
| :---- | :---- | :---- |
| **Adicionar** | **Botão.** | Adiciona um novo webhook do Slack. |
| **Nome do canal** | **Campo de texto.** | Adiciona o nome do canal. |
| **URL** | **Campo de texto.** | Adiciona a URL do webhook. |
| **Notification type** | **Menu suspenso.** | Seleciona os tipos de notificações para receber através do Slack. |
| **O que posso fazer aqui?** | **Botão.** | Acessa a documentação relacionada a esta tela. |
| **Ativar** | **Botão *toggle*.** | Ativa ou desativa a integração. |
| **Editar** | **Botão.** | Edita a integração. |