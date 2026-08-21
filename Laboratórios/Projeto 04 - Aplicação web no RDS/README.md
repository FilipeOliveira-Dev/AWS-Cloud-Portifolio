# 🖥️ Projeto 04 - Aplicação web no RDS


## 🌐 Visão Geral
Este é o projeto do Laboratório 04, de Criar um servidor de banco de dados e interagir com o banco de dados usando um aplicativo. O objetivo prático é implementar uma arquitetura de banco de dados relacional totalmente gerenciada e escalável na nuvem, utilizando o **[Amazon RDS (Relational Database Service)](https://aws.amazon.com/pt/products/databases)**.

Em ambientes corporativos, gerenciar servidores de banco de dados locais exige um esforço massivo com manutenção de hardware, patches de segurança, backups manuais e alta disponibilidade.
Ao delegar essa infraestrutura para o Amazon RDS, automatizamos essas tarefas administrativas demoradas. Isso garante tolerância a falhas e capacidade redimensionável de forma econômica, permitindo focar puramente no desenvolvimento do aplicativo e nas regras de negócio.


## ⚙️ Arquitetura do Projeto
A infraestrutura foi desenhada seguindo as melhores práticas de isolamento de rede, segurança granular e alta disponibilidade estruturada nas seguintes etapas:
- <b>Camada de Segurança:</b> Criação de um Security Group exclusivo para o banco de dados, configurado com regras rígidas de entrada que limitam o tráfego na porta padrão apenas para o Security Group do servidor web, bloqueando qualquer acesso externo direto da internet.
- <b>Segregação de Rede:</b> Configuração de um DB Subnet Group (Grupo de Sub-redes de Banco de Dados), delimitando as sub-redes privadas em diferentes Zonas de Disponibilidade (Multi-AZ) onde o banco de dados pode residir.
- <b>Provisionamento Gerenciado:</b> Execução de uma instância de banco de dados do Amazon RDS configurada para alta disponibilidade, garantindo failover automático e resiliência de dados em caso de falha de uma zona.
- <b>Consumo e Integração:</b> Conexão de um aplicativo web ativo à instância do RDS através do endpoint gerado, realizando interações diretas (leitura e escrita de dados) para validar o fluxo síncrono e a persistência da aplicação em produção.


## 🎬 Cenário final
Ao final do laboratório, essa será a infraestrutura:

<img width="800" height="400" alt="image" src="https://media.licdn.com/dms/image/v2/D4E22AQHEfqoipSvdow/feedshare-image-high-res/B4EZzdSxllJ4AU-/0/1773239212841?e=1785369600&v=beta&t=acSI2EPnAf9CO7phefR1lFBx36woaF3aKOJ5RGcQ3gw" />


## 📝 Tópicos Abordados

- Alta Disponibilidade (Multi-AZ): Provisionamento de uma instância de banco de dados com uma réplica secundária em uma Zona de Disponibilidade (AZ) distinta
- Segurança e Conectividade: Configuração de Security Groups específicos para permitir que apenas o servidor web (EC2) se comunique com o banco de dados
- Interação Full-Stack: Deploy de uma aplicação web para interagir em tempo real com os dados armazenados no MySQL Community
- Monitoramento: Utilização do Amazon CloudWatch para acompanhar métricas críticas como uso de CPU e balanço de créditos da instância


## 🛠️ Implementação Prática
> 1. <b>Criar um grupo de segurança para a instância de banco de dados do RDS</b>
> 2. <b>Criar um grupo de sub-redes de banco de dados </b>
> 3. <b>Criar uma instância de banco de dados do Amazon RDS</b>
> 4. <b>Interagir com o seu banco de dados</b>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-amazonrds-cloudcomputing-activity-7437504332151033856-gg4Q?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**



## 🏁 Conclusão
A conclusão deste projeto consolida o entendimento prático sobre a entrega de soluções Cloud Native robustas e seguras. A separação estrita entre a camada de aplicação (Web Server) e a camada de dados (RDS) demonstra o domínio sobre arquiteturas de múltiplas camadas (Multi-Tier Architectures).

Ao final do laboratório, o ecossistema comprovou estar totalmente funcional, seguro contra acessos não autorizados por meio de grupos de segurança interconectados e preparado para suportar oscilações de carga com redundância multi-zona.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>