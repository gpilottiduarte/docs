# Política de proteção de dados

## Segurança e privacidade de dados

O ambiente de nuvem que hospeda o senhasegura Private SaaS é protegido por um serviço de detecção de ameaças. Este serviço monitora constantemente ações prejudiciais ou atividades não autorizadas.

Além disso, cada cliente possui sua própria **Virtual Private Cloud (VPC)** dedicada. Isso garante que os dados de diferentes clientes permaneçam integralmente separados dentro do sistema, eliminando a possibilidade de erros de configuração, vazamentos de dados ou que a ação de um cliente afete outro.

O acesso à instância do senhasegura é restrito exclusivamente à rede do cliente. Isso significa que até mesmo a equipe de suporte do senhasegura deve se comunicar com o cliente para realizar ações que envolvam potencial exposição de dados. 

Termos de confidencialidade vinculam contratualmente nossos membros da equipe. Essas obrigações são reforçadas por meio de programas abrangentes de integração e treinamento periódico de reciclagem centrados em segurança da informação e conformidade com a GDPR.

Em situações em que o time de suporte precisar acessar o console de um cliente, a aprovação explícita e específica do cliente é obrigatória. É importante observar que cada instância de acesso fica registrada para futuras auditorias.

A ISO 27001O certificou as políticas e procedimentos operacionais implementados pelo senhasegura para prevenir erros. Em caso de violação, estamos comprometidos em informar prontamente o cliente, em conformidade com nossas obrigações legais.


* * *

## Backup
Todos os dias, às 3h GMT-3, o senhasegura tira snapshots do sistema. Por padrão, os snapshots dos últimos cinco dias são mantidos.

Os snapshots armazenam uma imagem completa de toda a aplicação. Dessa forma, se houver um problema e o sistema ficar indisponível, será possível restaurá-lo ao normal.

Tirar snapshots, manter o sistema atualizado e restaurá-lo em caso de problema são responsabilidades do senhasegura.

Se você preferir manter cópias de backup do aplicativo, vídeos e credenciais em seus dispositivos pessoais, lembre-se que você deve gerenciar os aspectos de segurança, controlar quem pode acessar esses backups e garantir espaço de armazenamento suficiente disponível.

* * *


## Coleta de dados

As seguintes informações são as únicas informações não públicas (NPI) e informações pessoalmente identificáveis (PII) que o senhasegura SaaS coleta para fornecer o serviço:


**Informações coletadas de dispositivos**: 

* Nome do computador.
* Endereço MAC do computador.
* Nomes de usuários e grupos.
* Usuário atualmente logado.
* Endereços IP do endpoint.
* Endereço IP usado para se conectar ao SaaS.
* Programas instalados.
* Detalhes sobre aplicativos lançados, conforme definido pelas políticas.
* Vídeos de captura de tela das sessões.

**Informações coletadas de usuários**: 

* Nome completo.
* Nome de usuário no SaaS.
* Senha.
* Endereço de e-mail.
:::(Info) (Info)
Os administradores têm a capacidade de anonimizar os dados do usuário por meio da interface web do senhasegura, garantindo conformidade com o requisito de direito ao esquecimento.
:::


* * *

## Retenção de dados
O período pelo qual o senhasegura mantém seus dados depende da quantidade de espaço de armazenamento disponível em seu pacote escolhido.

* * *

## Período de carência
Após o vencimento da licença, o acesso à interface web do senhasegura ainda estará disponível por duas semanas (contadas após o vencimento da licença), para que os clientes possam extrair seus dados adequadamente.

Em seguida, a instância será desligada, e as capturas de snapshot serão armazenadas por três meses (contados após o vencimento da licença).

* * *

## Extração de dados
Sempre que os clientes alteram suas senhas, é automaticamente criado um backup de suas credenciais. Esse backup é armazenado na rede do cliente, garantindo que a versão mais atualizada esteja sempre disponível localmente.

Os clientes também têm a opção de criar automaticamente backups locais das gravações de sessões. Além disso, eles podem acessar o senhasegura para extrair individualmente essas gravações.

:::(Error) (Importante)
Uma vez que os dados são extraídos, o cliente se torna totalmente responsável pela segurança e gerenciamento desses dados ao longo de seu ciclo de vida.
:::


* * *

## Procedimento de exclusão de dados

O processo de exclusão de dados será iniciado em uma das seguintes circunstâncias:

* Automaticamente, três meses após a data de término ou não renovação do contrato.
* Em resposta a uma solicitação específica por escrito do cliente ao senhasegura para a exclusão de dados.

Ao acionar o processo de exclusão de dados, a equipe do senhasegura seguirá os seguintes passos:

1. A máquina virtual do cliente será destruída.
2. Todos os dados relacionados ao cliente serão permanente e irreversivelmente excluídos de nossa nuvem em poucas horas.

:::(Error) (Importante)
Este processo de exclusão é registrado para fins de auditoria, possibilitando ao cliente solicitar a revisão do procedimento quando desejar.

:::

Durante todo o processo, o cliente receberá duas notificações:

* Notificação do desligamento da instância.
* Notificação confirmando que todos os dados foram completamente excluídos.

* * *

## Prazo para exclusão de dados
A nuvem do senhasegura depende da política de exclusão da Google Cloud, projetada para equilibrar a necessidade de alto desempenho com a exigência de exclusão oportuna de dados. Aqui está uma visão geral do cronograma de exclusão de dados:

1. Quando uma solicitação de exclusão é feita, os dados são marcados para exclusão imediata. O objetivo é concluir esse processo de marcação no período máximo de 24 horas. Após a marcação para exclusão, pode haver um período de recuperação interno de até 30 dias, dependendo do serviço específico ou da solicitação de exclusão.
2. Com os dados marcados para exclusão, eles passam por processos como a coleta de lixo para alcançar a exclusão lógica dos sistemas ativos. A execução desses processos varia conforme a replicação de dados e os ciclos contínuos de coleta de lixo. Geralmente, leva cerca de dois meses desde a solicitação para excluir de fato os dados dos sistemas ativos. Esse período permite a conclusão de dois ciclos significativos de coleta de lixo para garantir a exclusão lógica.

3. O ciclo de backup do Google garante que os dados excluídos nos backups dos centros de dados expirem dentro de seis meses. Dependendo da replicação de dados e do cronograma de backup do Google, os backups podem ser excluídos mais cedo.

Para informações detalhadas sobre o processo de exclusão da Google, acesse a [documentação do Google Cloud](https://cloud.google.com/docs/security/deletion?hl=pt-br){target="_blank"}. 

