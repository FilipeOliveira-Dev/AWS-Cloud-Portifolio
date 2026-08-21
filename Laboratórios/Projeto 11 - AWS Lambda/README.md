# 🖥️ Projeto 11 - AWS Lambda

## 🌐 Visão Geral
Neste laboratório, nós implantamos e configuramos uma solução de computação sem servidor baseada no **[AWS Lambda](https://aws.amazon.com/pt/pm/lambda/)**. A função do Lambda vai gerar um relatório de análise de vendas, extraindo dados de um banco de dados e enviando os resultados diariamente.<br>
As informações de conexão do banco de dados são armazenadas no armazenamento de parâmetros, um recurso do **[AWS Systems Manager](https://aws.amazon.com/pt/systems-manager/)**. O próprio banco de dados é executado em uma instância do Linux do Amazon Elastic Compute Cloud (Amazon EC2) **[Amazon Elastic Compute Cloud (Amazon EC2)](https://aws.amazon.com/pt/pm/ec2/)**, do Apache, do MySQL e do PHP (LAMP).


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEz2-9LGznPcQ/feedshare-image-high-res/B4DZ0GjW_DKoAU-/0/1773931426372?e=1788998400&v=beta&t=egX_4_eQiedZmqVrt4RvC0jqoNtufC5p-r-WyEZ9DGE" />


## 📝 Tópicos Abordados

- <b>Arquitetura de Duas Camadas:</b> Uma função Lambda principal coordena o fluxo, invocando uma segunda função especializada na extração de dados de um banco de dados MySQL (EC2 LAMP).
- <b>Lambda Layers:</b> Utilizei camadas para gerenciar a biblioteca externa PyMySQL, promovendo o reuso de código e mantendo as funções leves.
- <b>Segurança e Governança:</b> Armazenamento seguro de credenciais de banco de dados no AWS Systems Manager Parameter Store e gerenciamento refinado de permissões via IAM Roles.
- <b>Automação de Agendamento:</b> Implementação de gatilhos via EventBridge (CloudWatch Events) usando expressões Cron para disparos programados.
- <b>Notificações em Tempo Real:</b> Integração com Amazon SNS para entrega imediata dos relatórios processados via e-mail.


## 🛠️ Implementação Prática
> 1. <b>Observar as configurações do perfil do IAM</b>
> - <i>Etapa 1: Observar as configurações do perfil do IAM 'salesAnalysisReport' e 'salesAnalysisReportDERole'</i>
> 2. <b>Criar uma camada do Lambda e uma função extratora de dados do Lambda</b>
> - <i>Etapa 1: Criar uma camada do Lambda</i>
> - <i>Etapa 2: Criar a função extratora de dados do Lambda</i>
> - <i>Etapa 3: Adicionar a camada do Lambda à função</i>
> - <i>Etapa 4: Importar o código da função extratora de dados do Lambda</i>
> - <i>Etapa 5: Definir configurações de rede para a função </i>
> 3. <b>Testar a função extratora de dados do Lambda</b>
> - <i>Etapa 1: Iniciar um teste da função do Lambda</i>
> - <i>Etapa 2: Solucionar problemas da função extratora de dados do Lambda</i>
> - <i>Etapa 3: Fazer um pedido e testar novamente </i>
> 4. <b>Configurar notificações</b>
> - <i>Etapa 1: Criar e Assinar um tópico do SNS</i>
> 5. <b>Criar a função do Lambda salesAnalysisReport</b>
> - <i>Etapa 1: Conectar-se à instância CLI Host</i>
> - <i>Etapa 2: Configurar a AWS CLI</i>
> - <i>Etapa 3: Criar a função do Lambda salesAnalysisReport usando a AWS CLI</i>
> - <i>Etapa 4: Testar a função do Lambda salesAnalysisReport</i>
> - <i>Etapa 5: Adicionar um gatilho à função do Lambda salesAnalysisReport </i>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-lambda-serverless-activity-7440407688355688451-VBXB?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGRg7K-mXGvzQ/feedshare-image-high-res/B4DZ0GjW.WHcAU-/0/1773931426659?e=1788998400&v=beta&t=QY6sOHDgvPjn_VFi8-1HoPbPyYzRs8lPWx5MZzwAqMA" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQH0H9BSYWZwpw/feedshare-image-high-res/B4DZ0GjXDEKoBI-/0/1773931427033?e=1788998400&v=beta&t=qg4Kn9EAtkppxft1UBpMnuddu2KWbO84yags0LiM1Do" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGRd4YvPOAalg/feedshare-image-high-res/B4DZ0GjXB9KUAU-/0/1773931426756?e=1788998400&v=beta&t=Y2_rp0y-sUKaOtYevpcNFV7J8-ilNQNUgC3Eb0UQolM" /> 



## 🏁 Conclusão
A conclusão desta atividade valida o domínio sobre arquiteturas serverless modulares e padrões de automação operacional (SysOps/DevOps) na AWS.<br>
A implementação comprova como conectar serviços sem servidor a recursos tradicionais de computação e banco de dados de maneira segura, desacoplada e sem sobrecarga administrativa de servidores. Além disso, a configuração de camadas do Lambda para bibliotecas externas, a orquestração por agendamento cron e o uso do CloudWatch Logs para diagnóstico de execução preparam uma base sólida para criar pipelines eficientes de processamento de dados e alertas em ambientes de produção corporativos.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>