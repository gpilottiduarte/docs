# Notification Options

:::(info) (Info)
Para configurar notificações acesse: Registrar envio de notificação de operação
:::

## Backup de senha

-    **Backup Efetuado:**  Um backup de informações privilegiado foi feito usando a chave mestraEssa execução de backup pode ser executada por automação do sistema ou manualmente por solicitação do usuário

-    **Erro no Backup:** Ocorreu um erro durante um backup de informações privilegiadas

## Credenciais

-   **Senha Visualizada:** Quando uma senha for visualizada por um usuário

-   **Senha Alterada:** Alguma credencial tem senha alterada manualmente ou por modelo de módulo de execução

-   **Senha Expirada:** Um relatório com credenciais que tiveram as senhas expiradas

-   **Resumo Diário de Senhas:** Um relatório com resumo de operações de credenciais

-   **Senha Confirmada:** Um relatório com credenciais com senhas confirmadas

-   **Senha Inválida:** Um relatório com credenciais com senhas inválidas

-   **Configurações de dono da credencial:** Alguma credencial foi criada ou alterada para ter um proprietário dedicado

## Informações Protegidas

Operações de informação protegidas pelo PAM.

-   **Informação Visualizada:** Alguns usuários solicitaram dados de uma informação protegidas. Este usuário teve acesso à senha, arquivo ou conteúdo

-   **Informação Alterada:** Algumas informações protegidas foram alteradas

-   **Informação Expirada:** Algumas informações protegidas expiraram

## Equipamentos

Monitoramento de dispositivos PAM.

-   **Perda de Conectividade:** Dispositivos que perderam conectividade nas portas configuradas

-   **Conectividade Restabelecida:** Dispositivos que a conectividade de recuperação foi sinalizada como conectividade perdida

## Comandos auditados

Execução auditada do comando da sessão do proxy do SSH.

-   **Comando Detectado - Criticidade Baixa:** Algum usuário tentou executar um comando auditado configurado com pontuação baixa

-   **Comando Detectado - Criticidade Média:** Algum usuário tentou executar um comando auditado configurado com pontuação média

-   **Comando Detectado - Criticidade Alta:** Algum usuário tentou executar um comando auditado  configurado com pontuação alta

-   **Comando Detectado - Bloquear e interromper sessão:** Algum usuário tentou executar um comando auditado configurado para ser bloqueado. A sessão foi imediatamente interrompida

-   **Comando Detectado - Bloquear:** Algum usuário tentou executar um comando auditado configurado para ser bloqueado

-   **Comando Detectado - Permitir:** Algum usuário executou um comando auditado

## Controle de acesso

Notificações do processo de workflowCada produto/módulo que tem a funcionalidade de workflow pode enviar este tipo de mensagem

-   **Solicitação Criada:** Um novo pedido de aprovação foi feito por um usuárioAprovadores receberão um e-mail com detalhes

-   **Solicitação Aprovada:** Algum usuário aprovador aceitou o pedido

-   **Solicitação Reprovada:** Algum usuário do aprovador rejeitou o pedido. O usuário receberá uma notificação com o motivo da desaprovação

-   **Solicitação Revogada:** Algum usuário do tipo aprovador revogou o pedido e o usuário que solicitou receberá uma notificação com o motivo da revogação

-   **Gerenciamento de aprovadores:** Um usuário foi cadastrado como aprovador

## Sessão remota

Operações de proxy senhasegura

-   **Sessão iniciada:** Uma sessão de proxy é iniciada

-   **Sessão Finalizada :** Uma sessão de proxy é concluída

-   **Arquivo de sessão modificado:** Uma sessão teve seu arquivo de origem de auditoria alterado

-   **Texto indexado da sessão:** O senhasegura terminou para indexar um texto de sessão de proxy.

-   **Gerar vídeo para download:** Algum usuário solicitou a geração de vídeo MP4

-   **Vídeo agendado para download:** A geração de vídeo solicitada terminou

-   **Sessão de alto risco:** Uma sessão foi identificada como de alto risco

## Operação de senhas

Operações de credenciais do PAM executadas pelo módulo de Execuções.

-   **Erro de troca:** Ocorreu um erro ao tentar alterar a senha no dispositivo de destino pelo módulo de execução

-   **Troca Executada:** Uma credencial tomou sua senha alterada no dispositivo de destino pelo módulo de execução

-   **Ativação Executada:** Uma credencial foi ativada no dispositivo de destino por módulo de execução

-   **Erro de Ativação:** Ocorreu um erro quando tentou ativar no dispositivo de destino pelo módulo de execução

## Monitoramento

Monitoramento de recursos da instância do servidor

-   **Relatorio diário de troca de senhas:** Um relatório com resumo de operações de credenciais.

-   **Pouco Espaço em Disco - Criticidade Baixa:** O armazenamento está sendo executado abaixo de 30% do espaço livre

-   **Pouco Espaço em Disco - Criticidade Média:** O armazenamento está sendo executado abaixo de 20% do espaço livre

-   **Pouco Espaço em Disco - Criticidade Alta:** O armazenamento está sendo executado abaixo de 10% do espaço livre

-   **Espaço em Disco - Notificação diária:** Relatório diário de uso de armazenamento

-   **Uso de CPU - Alto:** A CPU está executando mais de 70% de uso durante 10 minutos.

-   **Uso de CPU - Crítico:** A CPU está executando mais de 90% de uso ao longo de 10 minutos.

-   **Consumo de memória - Crítico:** A RAM está funcionando com mais de 90% de uso em 10 minutos.

-   **Consumo de memória - Alto:** A RAM está rodando mais de 70% de uso em 10 minutos.

-   **O usuário baixou o PDF com o painel do sistema:** Algum usuário baixou um painel como PDF. Este alerta existe para deixar claro que alguns dados exportados por algum usuário

## Audit trail

Mudanças nas principais entidades registros.

-   **Audit trail:** Quando uma entidade é criada, atualizada ou inativada, um log detalhado é registrado e também pode ser notificado

## Autenticação

Mensagens do processo de autenticação

-   **Este usuário irá ignorar o uso de MFA:** Quando está desabilitado o uso de MFA

-   **Mensagens de autenticação:** Quando um usuário é autenticado ou alguma falha do processo de autenticação ocorre

-   **O uso de MFA não ignorado para este usuário:** Quando o uso de MFA está habilitado

## Workstation

senhasegura.go para Windows ou Linux.

-   **Aplicação iniciada:** Uma execução de aplicativos imparcionada iniciada

-   **Aplicação finalizada:** Uma execução de aplicação imparcial terminou

-   **Uso credencial para acesso a rede:** Uma credencial foi usada para acessar um compartilhamento de rede

-   **Nova versão do senhasegura.go:** Uma nova versão de senhasegura.go está disponível na senhasegura BackOffice

-   **Versão do senhasegura.go aprovada:** O instalador do MSI foi aprovado pelo administrador a ser instalado automaticamente do Cliente senhasegura.go

-   **Versão do senhasegura.go inativada:** O instalador do MSI foi rejeitado pelo administrador para ser instalado automaticamente do cliente senhasegura.go

-   **Download de versão do senhasegura.go realizada:** O cliente senhasegura.go baixou uma nova versão do backoffice

-   **Versão do senhasegura.go instalada:** Alguma estação de trabalho instalou a nova versão e relatou ao backoffice

-   **Workstation aprovada:** A estação de trabalho foi aprovada para usar senhasegura.go 

-   **Cadastro de workstation:** A estação de trabalho solicitou autorização para usar senhasegura.go

-   **Utilização do UAC:** O usuário usou senhasegura.go para autenticar o prompt do Windows UAC

-   **Visualizar senha:** O usuário visualizou a senha de credencial como texto simples

-   **Copiar senha:** Uma senha de credenciais foi copiada

-   **Runas:** Uma execução de aplicativos imparcionada iniciada no menu de contexto do Windows.

-   **Macro:** Uma macro foi executada por algum usuário

-   **Painel de controle:** Um applet de painel de controle representado foi acessado

-   **Adaptador de rede:** Um applet de configurações do adaptador de rede foi acessado por algum usuário

-   **Compartilhamento de rede:** Um caminho de compartilhamento de rede foi registrado por algum usuário

-   **Desinstalação:** O usuário desinstalou algum aplicativo usando senhasegura.go Elevation

-   **Ficar  online:** O usuário solicitou para parar o modo online senhasegura.go

-   **Ficar offline:** O usuário solicitou para iniciar o modo Offline do senhasegura.go

-  **Alerta:** As mensagens de alerta do sistema relacionadas a erros

-   **Erro ao buscar credenciais:** Ocorreu um erro quando o cliente senhasegura.go tentou solicitar a lista de credenciais do usuário

-   **Verificação de diretório e arquivo - Inclusão:** O diretório e a digitalização de arquivos adicionaram algumas políticas de permissão com base na configuração de backoffice

-   **Verificação de diretório e arquivo - Exclusão:** O diretório e a digitalização de arquivos removem algumas políticas de permissão com base na configuração de backoffice

-   **Verificação de diretório e arquivo - Alterar:** O diretório e a digitalização de arquivos alterou algumas políticas de permissão com base na configuração de backoffice

-   **Análise de malware de aplicações:**

-   **DLL não confiável:** O usuário tentou executar um programa que possui uma DLL considerada não confiável

## Certificates Manager

Mensagens do módulo do Gerenciador de Certificados.

-   **Alerta de expiração do certificado: Hoje:** Alguns certificados irão expirar hoje

-   **Alerta de expiração do certificado: 1 dia	:** Alguns certificados irão expirar em 1 dia

-   **Alerta de expiração do certificado: 7 dias:** Alguns certificados irão expirar em 7 dias

-   **Alerta de expiração do certificado: 15 dias:** Alguns certificados irão expirar em 15 dias

-   **Alerta de expiração do certificado: 30 dias:** Alguns certificados irão expirar em 30 dias

-   **Alerta de expiração do certificado: 60 dias:** Alguns certificados irão expirar em 60 dias

-   **Alerta de expiração do certificado: 90 dias:** Alguns certificados irão expirar em 90 dias

-   **Criaçao de certificado:** Quando um certificado é criadoPode ser acionado por via automática ou importação manual

-   **Download:** Algum usuário fez o download um certificado gerido pelo senhasegura Este certificado pode ser válido e publicado, um antigo ou mesmo um certificado não utilizado

-   **Gerenciamento de certificado:** Mostra configurações realizados em um certificado

-   **Gerenciamento de perfil de publicação:** Uma configuração de perfil de publicação foi criada ou alterada

-   **Gerenciamento de request:** Uma solicitação de certificado CSR foi criada ou alterada

-   **Renovação de certificado:** Um certificado foi renovado em dispositivos alvos

-   **Revogação de certificado:** Um certificado foi revogado em dispositivos alvos

-   **Visualização de senha de certificado:** Algum usuário visualizou a senha do certificado em texto simples

-   **Visualização de senha de request:** Uma senha de solicitação de certificado CSR foi visualizada

-   **Vínculo de certificado com dispositivo:** Quando um certificado é configurado em um dispositivo

## Comportamento

Comportamentos incomuns detectados pelo módulo de comportamento do usuário

-   **Acesso em horário incomum:** Uma sessão de proxy com um tempo de início incomum para esse usuário ou credencial

-   **Acesso de origem incomum:** Uma sessão de proxy começou por algum usuário de uma origem incomum para esse usuário ou credencial

-   **Acesso com duração incomum:** Uma sessão de proxy com um tempo de duração incomum para esse usuário ou credencial

-   **Visualização credencial incomum:** Algum usuário está solicitando uma visão de texto simples de uma credencial incomum para ele

-   **Visualização de origem incomum:** Algum usuário está solicitando visão simples de um IP de origem incomum

-   **Alteração de senha incomum:** Algum usuário realizou uma alteração na senha considerada incomum

-   **Acesso em destino incomum:** Uma sessão de proxy começou por algum usuário tentando acessar um destino incomum para esse usuário ou credencial

-   **Acesso de credencial incomum:** Algum usuário está tentando acessar uma credencial que é considerado incomum para aquele perfil de usuário

## Domum

-   **Nova localização:** Quando uma sessão for realizada em uma localização nova

-   **Localização inesperada:** Quando uma sessão é realizada de uma localização muito diferente do habitual ela é considerada inesperada

-   **Botão de pânico:** Quando o botão de pânico foi acionado

-   **Verificação de integridade do Domum:** Status sobre a integridade do acesso ao Domum


## Cloud

-   **Sessão IAM sem proprietário:** Quando uma sessão em uma conta cloud não tem propretário

-   **Visualização de chave IAM sem proprietário:** Quando ocorre uma visualização de chave IAM em uma conta cloud que não tem propretário

## Chave Mestra

-   **Tentativa de recuperação com falha:** Quando o usuário tenta recuperar o backup e acontece um erro

-   **Tentativa de recuperação com sucesso:** Quando o usuário recuperou o backup com sucesso


## Agendamento de relatórios

-   **Agendamento de relatórios - Criação:** Quando um agendamento de relatório foi criado

-   **Agendamento de relatórios - Atualização:**  Quando um agendamento de relatório foi atualizado

-   **Agendamento de relatórios - Exclusão:**  Quando um agendamento de relatório foi excluído

## Painel de emergência

-   **Botão de emergência:** Quando o botão de emergência foi acionado

-   **Lockdown iniciado:** Quando o Lockdown foi iniciado no sistema

-   **Lockdown finalizado:** Quando o Lockdown foi finalizado no sistema

-   **Freezing iniciado:** Quando o Freezing foi iniciado no sistema

-  **Freezing finalizado:** Quando o Freezing foi iniciado no sistema