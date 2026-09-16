# 🖥️ Projeto 19 - Monitorando a Infraestrutura

## 🌐 Visão Geral

Neste laboratório prático, nós exploramos a implementação de monitoramento contínuo, governança e visibilidade de infraestrutura na AWS. Nós utilizamos o AWS Systems Manager Run Command para implantar o agente do CloudWatch em instâncias Amazon EC2 de forma padronizada. 

Ao longo das tarefas, nós configuramos a coleta de métricas de sistema e logs de aplicações com o Amazon CloudWatch Logs e CloudWatch Metrics, aplicando filtros e alarmes para identificar eventos críticos. Além disso, nós estabelecemos respostas reativas em tempo real utilizando o Amazon EventBridge (CloudWatch Events) e garantimos o acompanhamento da conformidade técnica e dos padrões organizacionais através do AWS Config.



## 📝 Tópicos Abordados

- <b>Observabilidade com CloudWatch Agent:</b> Utilizei o Systems Manager Run Command para realizar o deploy em massa do agente do CloudWatch, permitindo a coleta de métricas de sistema (memória, disco) e logs de aplicação (Apache).
- <b>Análise de Logs e Filtros Métricos:</b> Configurei filtros no CloudWatch Logs para identificar padrões de erro (como o código HTTP 404) e transformá-los em métricas acionáveis, disparando alarmes automáticos via Amazon SNS.
- <b>Notificações em Tempo Real:</b> Implementei regras no CloudWatch Events (EventBridge) para detectar mudanças de estado na infraestrutura (instâncias paradas ou terminadas) e enviar alertas instantâneos via JSON.
- <b>Governança com AWS Config:</b> Ativei regras de conformidade para auditar automaticamente o ambiente, identificando recursos sem tags obrigatórias ou volumes EBS órfãos que gerariam custos desnecessários.


## 🛠️ Implementação Prática

> 1. <b>Instalar o agente do CloudWatch</b>
> 2. <b>Monitorar logs da aplicação usando o CloudWatch Logs</b>
> - <i>Etapa 1: Criar um filtro de métrica no CloudWatch Logs</i>
> - <i>Etapa 2: Criar um alarme usando o filtro</i>
> 3. <b>Monitorar métricas de instância usando o CloudWatch</b>
> 4. <b>Criar notificações em tempo real</b>
> - <i>Etapa 1: Configurar uma notificação em tempo real</i>
> 5. <b>Monitorar a conformidade da infraestrutura</b>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudwatch-awsconfig-activity-7448026577000468481-UBcp?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEaLc19eQyb7A/feedshare-image-high-res/B4DZ1y0sowHMAU-/0/1775747911151?e=1791417600&v=beta&t=NeqyUvSHheJkH1Xy01O5EWZaMxyKP8Rl5N7OpBXbmgo" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHCRVrENN9Nsw/feedshare-image-high-res/B4DZ1y0stXGUAY-/0/1775747911344?e=1791417600&v=beta&t=1uWta48nPuEkxbOKh7khfvJiExLJauwABlNxQyXRVxk" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFHqJlOuW2BZQ/feedshare-image-high-res/B4DZ1y0ssWKUAU-/0/1775747911541?e=1791417600&v=beta&t=S-koM36remMdKEaAmSjxz0GxX4s-Z5g4GRI1PjszDZM" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e dominamos ferramentas fundamentais de observabilidade e governança na nuvem da AWS. Nós instalamos e configuramos o agente do CloudWatch via Systems Manager, permitindo o monitoramento detalhado de métricas de sistema e a centralização de logs de aplicações no CloudWatch Logs. 

Além disso, nós estruturamos filtros de métricas e alarmes para detecção de anomalias, configuramos eventos do EventBridge para automação de notificações em tempo real e aplicamos o AWS Config para auditar e manter a conformidade da infraestrutura de forma contínua.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>