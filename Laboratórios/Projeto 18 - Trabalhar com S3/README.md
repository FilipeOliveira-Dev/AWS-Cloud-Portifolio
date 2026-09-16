# 🖥️ Projeto 18 - Trabalhar com S3

## 🌐 Visão Geral

Neste laboratório prático, nós configuramos uma solução segura de compartilhamento de arquivos e monitoramento de eventos utilizando o **[Amazon Simple Storage Service (Amazon S3)](https://aws.amazon.com/pt/pm/serv-s3/)** e o **[Amazon Simple Notification Service (AWS SNS)](https://aws.amazon.com/pt/sns/)**. Nós nos conectamos a uma instância EC2 dedicada como ambiente CLI Host para administrar os recursos através da AWS CLI, utilizando comandos como s3 e s3api para a criação e inicialização do bucket. 

Durante as atividades, nós validamos as políticas de permissão do IAM para o usuário externo mediacouser, garantindo o princípio do menor privilégio no envio e gestão de imagens. Por fim, nós estabelecemos uma arquitetura reativa ao associar notificações de eventos do bucket ao tópico do SNS, assegurando que alterações de conteúdo disparassem alertas automáticos por e-mail para o administrador.


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHilxAvbAKUgg/feedshare-image-high-res/B4DZ1OlcE3IYAc-/0/1775139931092?e=1791417600&v=beta&t=NMizJJ9iVvX8toe1lepAzH7WYpazm364324cQpd2h4w" />


## 📝 Tópicos Abordados

- <b>Automação via AWS CLI:</b> Utilizei os comandos s3 e s3api para criar buckets, sincronizar diretórios de imagens e configurar políticas complexas diretamente pelo terminal.
- <b>Segurança e IAM:</b> Configurei permissões granulares para usuários externos (mediacouser), garantindo que pudessem gerenciar objetos (Get, Put, Delete) apenas em prefixos específicos (/images), sem acesso a configurações críticas do bucket.
- <b>Notificações Baseadas em Eventos:</b> Implementei uma integração onde o S3 publica eventos (ObjectCreated e ObjectRemoved) em um tópico do Amazon SNS, disparando alertas automáticos por e-mail para os administradores sempre que os dados são modificados.
- <b>Validação de Políticas:</b> Testei cenários de uso não autorizado, validando que as políticas de Least Privilege(Privilégio Mínimo) impediam tentativas de alteração de ACLs por usuários não administrativos.


## 🛠️ Implementação Prática

> 1. <b>Conectar-se à instância do EC2 CLI Host e configurar a AWS CLI</b>
> - <i>Etapa 1: Conectar-se à instância do EC2 CLI Host</i>
> - <i>Etapa 2: Configurar a AWS CLI na instância CLI Host</i>
> 2. <b>Criar e inicializar o bucket de compartilhamento do S3</b>
> 3. <b>Revisar as permissões do usuário e do grupo de usuários do IAM</b>
> - <i>Etapa 1: Analisar o grupo do IAM mediaco</i>
> - <i>Etapa 2: Analisar o usuário mediacouser do IAM</i>
> - <i>Etapa 3: Testar as permissões do mediacouser </i>
> 4. <b>Configurar notificações de eventos no bucket de compartilhamento do S3</b>
> - <i>Etapa 1: Criar e configurar o tópico do SNS s3NotificationTopic</i>
> - <i>Etapa 2: Adicionar uma configuração de notificação de eventos ao bucket do S3</i>
> 5. <b>Testar as notificações de eventos do bucket de compartilhamento do S3</b>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-amazons3-amazonsns-activity-7445476524092325889-__PR?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHF611nCXLllw/feedshare-image-high-res/B4DZ1Olb_MI4AU-/0/1775139930690?e=1791417600&v=beta&t=VVKSvD9IwaSEfPOxeZRy9jZI-kKdNAx3BMeNTDWQDe0" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGSUlf_8lW_Xg/feedshare-image-high-res/B4DZ1OlcE8IoAY-/0/1775139931389?e=1791417600&v=beta&t=5IIEN7cp0uQgT5XmcjnU9_UtpPnhvX3fK6gouUHynM8" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQF3U2H7jt42zA/feedshare-shrink_800/B4DZ1OlcBbG4Ag-/0/1775139930540?e=1791417600&v=beta&t=WuGi5f6MmqsxaQOjJ-iUGcNe4zQbHBDMXDgicHYL-XE" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e consolidamos habilidades essenciais para a automação e segurança no armazenamento em nuvem da AWS. Nós utilizamos os comandos s3api e s3 da AWS CLI para implantar e estruturar um bucket do Amazon S3, validando minuciosamente as permissões de gravação concedidas a usuários e grupos do IAM. 

Além disso, nós implementamos e testamos com sucesso a integração de notificações de eventos entre o S3 e o Amazon SNS, estabelecendo um fluxo automatizado de auditoria e monitoramento em tempo real para qualquer modificação realizada nos arquivos do bucket.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>