# FAQ

## Atualizações e Manutenção 

### Snapshots da instância

- **Quem é responsável por tirar snapshots da instância?**   
  - O senhasegura é responsável por tirar esses snapshots diariamente e antes da manutenção programada.

### Atualizações de Versão 

- **Como são realizadas as atualizações de versão?**   
  - No modelo SaaS, as atualizações são tratadas pelo suporte de acordo com a programação do fabricante. No modelo Private SaaS, as atualizações são coordenadas entre a equipe de suporte e o cliente.

## Arquitetura e backup 

### Snapshots Vs. backups regulares 

- **Por que são tirados snapshots em vez de backups regulares?**   
  - Os snapshots capturam uma imagem completa da aplicação, permitindo a restauração em caso de indisponibilidade ou incidente.

### Backup Local 

- **Por que há um backup local?**   
  - Backups locais permitem procedimentos de “*break the  glass*” sem necessidade de acesso à nuvem, garantindo acesso ao dispositivo durante a indisponibilidade.

### Armazenamento de Backup 

- **Onde são armazenadas as cópias de backup?**   
  - Backups de credenciais são armazenados na rede do cliente para procedimentos de "*break the glass*".

### Opções de Provedores de Nuvem

- **Posso usar outro provedor de nuvem?**   
  - A senhasegura define o provedor de serviços para o SaaS. Clientes que preferem outro provedor devem optar pela versão on-premises.

### Redundância e Recuperação de Desastres 

- **Há redundância entre diferentes regiões?**   
  - Por padrão, não. O senhasegura utiliza os serviços de contingência do Google para a disponibilidade dos dados. Arquiteturas multi-região requerem um contrato de serviço adicional.  
- **É possível ter uma instância de Recuperação de Desastres (DR) em outra nuvem?**   
  - Ambientes DR (Recuperação de Desastres) não são normalmente incluídos por padrão nas ofertas do senhasegura; eles envolvem custos extras e arranjos complexos.

### Arquitetura Ativo-Ativo 

- **Há uma arquitetura ativo-ativo disponível?**   
  - O ambiente do Google inclui sistemas de backup específicos por região. Serviços de backup entre regiões estão disponíveis separadamente.

### Configurações personalizadas de backup

- **É possível criar backups em outros provedores de nuvem?**   
  - Os clientes podem fazer backup de vídeos e credenciais em um servidor gerenciado pessoalmente, seja baseado em nuvem ou físico. Os snapshots diários do senhasegura são armazenados no GCP na mesma região que a instância.

## Regulamentos e segurança 

### Planos de contingência 

- **Qual é o plano de contingência em caso de falha na região hospedada?**   
  - Os múltiplos data centers do GCP em cada região garantem failovers transparentes, minimizando riscos de falha.

### Teste de intrusão 

- **Com que frequência são realizados testes de intrusão no ambiente da aplicação?**   
  - Testes de intrusão coincidem com cada atualização de software no ambiente de hospedagem, utilizando ferramentas padrão de mercado e consultores externos.

### Segurança dos dados 

- **O que garante que a máquina do cliente não será clonada ou copiada?**   
  - senhasegura emprega políticas operacionais abrangentes certificadas pela ISO 27001 para prevenir erros.

## Gerenciamento e acesso remotos

### Acesso de Suporte

- **Como o senhasegura fornece suporte remoto para clientes SaaS?**   
  - O acesso pela equipe do senhasegura é limitado à rede do cliente, com todas as atividades registradas para trilhas de auditoria.

### Acesso ao Painel Orbit

- **Há acesso ao painel Orbit no SaaS?**   
  - No novo modelo SaaS, apenas o senhasegura pode acessar o menu Orbit. Clientes têm acesso ao Orbit na configuração SaaS Privado.

## Gerenciamento de Backups 

### Responsabilidade pelos backups 

- **Quem gerencia os backups no SaaS e SaaS Privado?**   
  - No modelo SaaS, o senhasegura gerencia os backups do sistema, enquanto os backups de senhas são de responsabilidade do cliente via rsync. Clientes SaaS Privado gerenciam ambos os backups de sistema e senhas de forma independente.

