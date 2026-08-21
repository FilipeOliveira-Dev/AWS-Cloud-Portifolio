# 🖥️ Projeto 12 - [DESAFIO] AWS Lambda para contar palavras

## 🌐 Visão Geral

Esse laboratório de desafio tem como objetivo implementar uma arquitetura orientada a eventos (Event-Driven Architecture) totalmente sem servidor utilizando o AWS Lambda, o Amazon S3 e o Amazon SNS.
A solução automatiza o processamento assíncrono de dados: sempre que um novo arquivo de texto é enviado a um bucket do Amazon S3, o evento de upload (s3:ObjectCreated:*) dispara automaticamente uma função Lambda em Python.

A função executa a leitura do objeto, calcula a contagem total de palavras no texto e publica a mensagem formatada em um tópico do Amazon SNS, entregando os resultados diretamente por e-mail aos destinatários configurados.

A atividade enfatiza a integração nativa entre serviços de armazenamento, computação serverless e mensageria, utilizando políticas de privilégio mínimo e perfis do AWS IAM para governança segura dos recursos.


## 📝 Tópicos Abordados

- <b>Processamento com AWS Lambda:</b> Desenvolvi uma função em Python capaz de interceptar eventos de upload, processar o conteúdo do arquivo e calcular a métrica desejada.
- <b>Gatilhos com Amazon S3:</b> Configurei o bucket para invocar automaticamente a função Lambda sempre que um novo arquivo de texto fosse carregado.
- <b>Notificação via Amazon SNS:</b> Integrei o serviço de mensageria para enviar o resultado do processamento ("Word Count Result") diretamente para o e-mail do administrador em tempo real.
- <b>Segurança e Governança:</b> Utilizei o perfil LambdaAccessRole para garantir que a função tivesse as permissões estritas necessárias para interagir com S3, CloudWatch e SNS.


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-lambda-serverless-activity-7442994388663947264-h1Rw?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHq9-oV-ZU2MA/feedshare-image-high-res/B4DZ0rT8z1HEAY-/0/1774548144227?e=1788998400&v=beta&t=n-Y7JSP0FfO8ptrLna4czCTtTfHCsfO66-sw_-FSrUI" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGv-dbEBRYJAQ/feedshare-image-high-res/B4DZ0rT80MGoAg-/0/1774548144626?e=1788998400&v=beta&t=HxIvG_BpRfSI90Yp4t7L7g4x9szje9jM_VQ-In74mRg" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGN7ajphqNvmw/feedshare-image-high-res/B4DZ0rT82MIAAY-/0/1774548144596?e=1788998400&v=beta&t=-PcdAU5IYphj_VSLLQoCIz0CAwbM3LYZhfu5Tm5IcrY" /> 
---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQG71FuJO1qjMw/feedshare-image-high-res/B4DZ0rT8zqJoAU-/0/1774548144168?e=1788998400&v=beta&t=jAZooeODZsTCCAaV-crGw_Wjr_pM96xs_avyPkMp8BE" /> 



## 🏁 Conclusão
A conclusão deste desafio consolida o domínio sobre o desacoplamento de serviços e o processamento de dados sob demanda na nuvem sem necessidade de gerenciar instâncias ou servidores ativos.

Ao integrar o acionamento automático do S3 com a lógica do AWS Lambda e as notificações do Amazon SNS, valida-se na prática o padrão moderno de arquiteturas reativas em tempo real. Essa abordagem demonstra eficiência de custos — já que a computação só é tarifada durante os milissegundos de execução do script —, além de alta escalabilidade e resiliência operacional para fluxos de trabalho e pipelines de ingestão de dados em ambientes de produção corporativos.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>