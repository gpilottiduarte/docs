# Como configurar uma credencial no senhasegura

Este tutorial é um guia passo a passo para configurar uma credencial no senhasegura. Certifique-se de atender  aos requisitos listados abaixo antes de prosseguir com as etapas de configuração.

## Requisitos

- Estar registrado/habilitado com o papel de PAM operator no senhasegura.
- Ter um dispositivo criado.

## Como configurar uma credencial

Existem duas maneiras de acessar a área de configuração de **Credenciais**.

A primeira maneira é pelo menu de **Ações Rápidas**, localizado na barra de ferramentas superior. Para configurar uma credencial utilizando as ações rápidas, siga os passos abaixo:

1. Clique no ícone **Ações Rápidas**, representado por uma folha de papel com o sinal de soma, e selecione **Credencial**.

A segunda maneira é acessando pelo Grid Menu. Para isso, siga os passos abaixo:

1. No canto superior esquerdo da plataforma do senhasegura, clique no **Grid Menu**, representado pelos nove quadrados, e selecione **PAM Core**.
2. No menu lateral, selecione **Credenciais > Todas.**
3. Clique no ícone **Exibir Ações**, representado pelos três pontos verticais, e clique em **+ Novo**.

Ambas ações abrirão uma nova janela pop-up que você deverá preencher com seus dados.

### Na aba Informações

1. **Nome do usuário.**
2. **Tipo de senha.**
3. **Domínio.**
4. **Dispositivo.**
5. **Informação adicional.**
6. Habilite a **Situação*** como **Ativa** ou **Inativa**, ****para categorizar o status.
7. Defina a senha da credencial (limite de 256 caracteres, 70 se a troca for automatizada).
8. Escolha gerar uma senha aleatória conforme a política de senha.
9. Opcionalmente, preencha as **Tags** para identificação da credencial.
10. Clique no botão **Salvar**.

### Na aba Configurações de execução

1. **Credencial pai**: escolha no menu suspenso a credencial pai. Atente-se que, ao escolher uma credencial pai, a credencial filha irá assumir a mesma senha da credencial pai. Sempre que ocorrer uma troca de senha, manual ou automatizada, na credencial pai, a credencial filha também será modificada e assumirá a mesma senha da credencial pai.
2. Na seção **Configuração de troca de senha da credencial:**
    1. **Ativar troca automática**: assinale essa caixa de seleção para tornar ativa a troca automatizada da senha da credencial.
    2. **Habilitar troca via agente:**
    3. **Plugin de troca:** escolha, no menu suspenso, o plugin para realizar a troca automatizada da senha da credencial.
    4. **Template de troca:** selecione, no menu suspenso, o template para realizar a troca automatizada da senha da credencial.
3. Na seção **Configuração de autenticação:**
    1. **Utilizar a própria credencial para conectar**: assinale essa caixa de seleção para utilizar a própria credencial para realizar autenticação.
    2. **Credencial de autenticação**: selecione, no menu suspenso, a credencial que realizará a autenticação.
4. Na seção **Configuração da credencial de reconciliação**, na opção **Situação**, selecione a opção Ativo ou Inativo. Esta opção habilita a reconciliação de credenciais. Para mais informações, acesse a documentação sobre Como reconciliar senha de credenciais.

### Na aba Configurações da sessão

1. **Conectividades**: selecione as opções de conectividade as quais essa credencial terá acesso.
2. Na seção **Configurações de aplicativo remoto**:
    1. **Restringir o acesso apenas para aplicativo remoto:** assinale essa caixa de seleção se você deseja que essa credencial tenha acesso apenas a um ou mais aplicativos remotos. Caso você marque a opção, vai ser preciso indicar quais aplicativos remotos serão acessados por essa credencial. Assim, preencha os campos abaixo:
        1. **Macro de automação (RemoteApp):** clique no botão de soma para adicionar os aplicativos que serão utilizados. Ao clicar no botão de soma você terá acesso a dois menus suspensos:
            1. **RemoteApp**: selecione, no menu suspenso, o aplicativo que deseja dar acesso à credencial.
            2. **Conectividade**: selecione o protocolo de conexão que esse aplicativo remoto utilizará.
    2. **Utilizar a própria credencial para conectar:** assinale essa caixa de seleção para utilizar a própria credencial para realizar autenticação.
    3. **Credencial de autenticação:** indique a credencial que será utilizada para autenticação.
    4. **Dispositivo de autenticação:** indique o dispositivo onde será realizada a autenticação.
3. Na seção **Certificado**:
    1. **Arquivo do certificado**: faça upload do arquivo do certificado.
    2. **Arquivo da chave**: faça upload do arquivo de chave (key) para autenticação.
    3. **Senha da chave:** senha do arquivo da chave.

:::(Error) (Alerta)
- O certificado só será utilizado quando você estiver cadastrando uma credencial para conectar-se a um banco de dados Oracle. Para mais informações, acesse a documentação sobre [Sessões Oracle](/v3-33/docs/pt/pam-session-oracle-sessions).
- Quando for feito o upload de um certificado, este vai ser atrelado à credencial no momento do upload. Atente-se, contudo, que caso você precise editar essa credencial após salvá-la, não haverá indicação de que foi feito o upload do arquivo de certificado.
- Se for necessário, é possível substituir o certificado, para isso apenas faça upload novamente do arquivo.
:::

### Na aba Configurações adicionais

1. **Identificador (para webservice)**: indique o identificador do webservice usado na credencial./
:::(Info) (Info)
Caso o campo **Identificador** seja deixado em branco durante a criação de uma credencial, o sistema atribui automaticamente um UUID (Identificador Único Universal) a ela. O UUID gerado será então exibido no campo **Identificador** na interface. Caso deseje, você pode alterar esse valor para um de sua preferência. 
:::
2. **Usuário dono da credencial**: define o dono da credencial, o usuário que for indicado nesse campo será o único com acesso a credencial.
3. **Caminho no servidor**: esse campo é utilizado para especificar a localização da credencial nos arquivos. Essa funcionalidade é particularmente útil em situações em que há a necessidade de alterar a senha nos arquivos. Ao fornecer o caminho é possível identificar com precisão onde realizar a troca da credencial no servidor.
4. **Secret key (TOTP):** preencha com a sua chave TOTP. Para mais informações, [acesse a documentação sobre como gerar um Token OTP](/v3-33/docs/pt/pam-how-to-generate-a-totp-authentication-token).

:::(error) (Alerta)
Para o devido funcionamento da funcionalidade de TOTP, a sua chave secreta deve ser inserida em caixa alta (letras maiúsculas).
:::

5. Na seção **Campos adicionais para autenticação:**
    1. **Novo campo extra:** ao clicar no sinal de soma, você poderá cadastrar parâmetros adicionais para a autenticação. No caso você poderá passar os seguintes parâmetros: *Nome, Apelido e Valor.*
    2. **Observações**: preencha com observações pertinentes, caso necessário.

:::(Warning) (Importante)
- O limite de credenciais varia conforme a licença contratada no senhasegura.
- A existência de uma credencial pai não impede que a senha da credencial filha seja alterada manual ou automaticamente.
:::

## Como editar uma credencial

Para editar uma credencial, siga os passos a seguir:

1. Na plataforma senhasegura, no canto superior esquerdo, clique em **Grid Menu**, representado pelos nove quadrados, e selecione **PAM Core**.
2. No menu lateral, selecione **Credenciais > Todas.**
3. Na listagem, identifique a credencial que deseja editar e, na coluna **Ação**, clique no ícone representado pelos três pontos verticais e selecione, no menu suspenso, a opção **Editar,** representada pelo ícone do lápis e papel.
4. Na janela **Cadastro de credencial**, edite as configurações que desejar, de acordo com as instruções deste documento.
5. Clique em **Salvar**.

***

## Próximos passos
1. [Como configurar uma credencial de reconciliação](/v3-33/docs/pt/pam-how-to-configure-a-reconciliation-credential).
2. [Como realizar a reconciliação de uma credencial](/v3-33/docs/pt/pam-how-to-reconcile-a-credential).
3. [Como utilizar a funcionalidade “bulk action” para credenciais](/v3-33/docs/pt/pam-how-to-use-the-bulk-action-feature-for-credentials).
4. [Como cadastrar uma credencial de aplicação](/v3-33/docs/pt/pam-how-to-register-an-application-credential).
5. [Como verificar o histórico de execuções de uma credencial](/v3-33/docs/pt/pam-how-to-verify-the-execution-history-of-a-credential).
6. [Como gerar um token de autenticação TOTP](/v3-33/docs/pt/pam-how-to-generate-a-totp-authentication-token).
7. [Relatórios de controle de acesso](/v3-33/docs/pt/pam-access-control-reports-reference).
8. [Referência para credenciais](/v3-33/docs/pt/pam-reference-for-credentials).
9. [Referência sobre gerenciamento de credencial](/v3-33/docs/pt/pam-credential-management-reference).

***

Você ainda tem dúvidas? Entre em contato com a [Comunidade senhasegura](https://community.senhasegura.io/).