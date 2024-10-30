# Arquitetura

A arquitetura das soluções da senhasegura é projetada para oferecer opções flexíveis, seguras e escaláveis, atendendo às diversas necessidades dos clientes. Ao disponibilizar tanto o modelo **Private SaaS** quanto o modelo SaaS padrão, a senhasegura garante que as organizações possam escolher a arquitetura que melhor se adapte aos seus requisitos de segurança, conformidade e operações.

## Localização e segurança do data center

A aplicação SaaS da senhasegura é operada a partir dos data centers seguros do Google, que possuem certificação SOC 2 Tipo II e SOC 3 Tipo II. Esses centros estão equipados com sistemas robustos de backup de energia, mecanismos de supressão de incêndios e segurança 24 horas por dia. O acesso físico às salas de servidores é altamente restrito, garantindo um controle rigoroso contra intrusões.

Para cumprir com regulamentos locais, como o GDPR, e respeitar a soberania nacional, o ambiente de cada cliente é hospedado em servidores geograficamente próximos, assegurando conformidade e desempenho com baixa latência.

### Disponibilidade geográfica para SaaS

* **Brasil**  
* **EUA (Em breve)**  
* **Europa (Em breve)**  
* **Oriente médio (Em breve)**

### Disponibilidade geográfica para Private SaaS 

* **Qualquer região oferecida pelo GCP (Google Cloud Platform), [verifique aqui todas as regiões disponíveis](https://cloud.google.com/about/locations/#lightbox-regions-map).**

## Comunicação e integração

Toda a comunicação entre a senhasegura e a rede corporativa do cliente é facilitada através do [Network Connector](https://docs.senhasegura.io/v3-33/docs/network-connector). Este conector é implementado como um contêiner que se integra perfeitamente à infraestrutura de rede existente do cliente.

---

## Arquitetura sem VPN

![image](https://cdn.document360.io/5a1d58df-64ce-42a2-8b23-688477d32f33/Images/Documentation/image-1689002215816.png){height="" width=""}

No modelo sem VPN, toda a conectividade dentro do ambiente do cliente é gerenciada através do Network Connector. As principais características incluem:

* A instância do senhasegura pode ou não ser acessível publicamente.  
* Os usuários acessam o senhasegura utilizando o endereço IP público do cliente.  
* Os clientes podem autorizar múltiplos endereços IP para acessar a interface gráfica do senhasegura.

**Nota**: As conexões com o senhasegura são realizadas via Internet. Se o cliente puder identificar os IPs públicos a partir dos quais as conexões serão feitas, podemos filtrar apenas esses IPs para aumentar a segurança. Isso inclui clientes com uma faixa de endereços IP contratados de seu provedor de serviço de internet ou aqueles que mapeiam cada IP de saída individualmente.

## Uso do Network Connector da senhasegura

A senhasegura disponibiliza o [Network Connector](/v3-33/docs/network-connector) que pode ser implementado dentro da infraestrutura do cliente. Este conector facilita diversas tarefas, como a troca remota de senhas, e atua como um proxy para conexões de acesso remoto de forma que possibilita a integração com outros serviços do cliente. O **Network Connector** é um componente crítico para manter a conectividade segura entre o ambiente do cliente e as soluções SaaS da senhasegura.

## Uso do senhasegura Go Endpoint Manager

Toda a comunicação com o senhasegura **Go Endpoint Manager** é realizada via `HTTPS`, garantindo conectividade segura. Os endpoints gerenciados precisam ter a capacidade de se conectar ao ambiente SaaS da senhasegura.
