# 🖥️ Projeto 13 - Migração para Amazon RDS

## 🌐 Visão Geral
Este laboratório prático tem como objetivo realizar a migração de um banco de dados relacional local para uma instância totalmente gerenciada no **[Amazon Relational Database Service (Amazon RDS)](https://aws.amazon.com/pt/route53/)**.<br>
Ao final, o endpoint da aplicação da cafeteria é reconfigurado para se conectar à nova instância gerenciada do RDS dentro da mesma VPC, elevando os padrões de segurança, escalabilidade e disponibilidade da infraestrutura.


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGiswOuFukZMw/feedshare-image-high-res/B4DZ01gN7OKAAU-/0/1774719131878?e=1788998400&v=beta&t=dTGhM8-gX_lZdd_xYml9OCHsOCpEIRc9NDe0GWllMXc" />


## 📝 Tópicos Abordados

- <b>Infraestrutura como Código (CLI):</b> Provisionei toda a infraestrutura necessária via AWS CLI, incluindo Subnet Groups privados em diferentes Zonas de Disponibilidade e Security Groups com regras restritivas de acesso.
- <b>Estratégia de Migração:</b> Utilizei o utilitário 'mysqldump' para realizar o backup lógico do banco local e o restaurei no endpoint do RDS, garantindo a integridade de todos os pedidos existentes.
- <b>Configuração Dinâmica:</b> Reconfigurei a aplicação sem alterar o código, apenas atualizando os parâmetros de conexão no AWS Systems Manager Parameter Store.
- <b>Monitoramento Ativo:</b> Implementei o acompanhamento de métricas críticas como 'CPU Utilization' e 'Database Connections' via Amazon CloudWatch, validando o desempenho em tempo real


## 🛠️ Implementação Prática

> 1. <b>Gerar dados de pedidos no site da cafeteria</b>
> 2. <b>Criar uma instância do Amazon RDS usando a AWS CLI</b>
> - <i>Etapa 1: Conectar-se à instância CLI Host</i>
> - <i>Etapa 2: Configurar a AWS CLI</i>
> - <i>Etapa 3: Criar componentes obrigatórios</i>
> - <i>Etapa 4: Criar a instância do MariaDB do Amazon RDS</i>
> 3. <b>Migrar dados da aplicação para a instância do Amazon RDS</b>
> 4. <b>Configurar o site para usar a instância do Amazon RDS</b>
> 5. <b>Monitorar o banco de dados do Amazon RDS</b>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-amazonrds-cloudcomputing-activity-7443711562248302592-Py9G?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQG1d0nfnR6bVg/feedshare-image-high-res/B4DZ01gN5uJQAU-/0/1774719131890?e=1788998400&v=beta&t=uQV-j3K2f-NGeRdWHg7EttH67L4meTilMjZYB-8MOUo" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGjPPA4ALfCAw/feedshare-image-high-res/B4DZ01gN7UIYAU-/0/1774719131853?e=1788998400&v=beta&t=KMtqYEwEmkBJfOM4dmx7E4tropq6cjS-mPF8urRY5c8" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHU40Wh7jfzaA/feedshare-image-high-res/B4DZ01gN6IKMAU-/0/1774719131848?e=1788998400&v=beta&t=UHfSULjdeCU5_NSvJxhscXN25n4XEJZqewctt-zew3U" /> 



## 🏁 Conclusão
A conclusão desta atividade valida o domínio sobre processos essenciais de modernização e migração de infraestrutura legada para arquiteturas em múltiplas camadas (Multi-Tier) na AWS.<br>
O desacoplamento do banco de dados local em favor do Amazon RDS elimina pontos únicos de falha, garante o isolamento da camada de persistência em sub-redes privadas não expostas à internet e reduz a sobrecarga operacional por meio de backups automatizados e manutenção gerenciada. Esse fluxo prático consolida competências fundamentais para o dia a dia DevOps/SysOps no suporte à escalabilidade e resiliência de aplicações corporativas em nuvem.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>