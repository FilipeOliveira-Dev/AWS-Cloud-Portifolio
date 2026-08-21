# 🖥️ Projeto 07 - Criar Site no S3


## 🌐 Visão Geral
Este laboratório prático aborda a utilização avançada da **[AWS CLI (Command Line Interface)](https://aws.amazon.com/pt/cli/)** a partir de uma **[instância Amazon EC2]( https://aws.amazon.com/pt/pm/ec2/)** para automatizar o provisionamento de recursos de armazenamento e segurança, culminando no deploy de um site estático.

A atividade foca na eliminação de processos manuais via Console de Gerenciamento, demonstrando como interagir de forma puramente programática com o  **[Amazon S3](https://aws.amazon.com/pt/pm/serv-s3/Amazon)** e o **[AWS IAM](https://aws.amazon.com/pt/iam/)**. O objetivo central é capacitar o operador a configurar ambientes de hospedagem web seguros, gerenciar permissões granulares de acesso e criar scripts de automação (shell scripting) que tornam as atualizações de infraestrutura eficientes, repetíveis e integradas às práticas modernas de DevOps.


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGCGvp9hYkL3A/feedshare-image-high-res/B4DZ0bIq1aIwAY-/0/1774276751086?e=1785974400&v=beta&t=CQNGDTGj8FOxRzEyS24VKWTuGpVo6q0XQvFt5f-ghSw" />


## 📝 Tópicos Abordados

- <b>Infraestrutura via CLI:</b> Criação de buckets S3 e configuração de usuários IAM com políticas específicas diretamente pelo terminal.
- <b>Hospedagem Estática:</b> Configuração de um bucket para servir como endpoint de site, definindo documentos de índice e permissões de acesso público (ACLs).
- <b>utomação com Bash Script:</b> Desenvolvi um script executável (.sh) para tornar a atualização do site repetível e eficiente.
- <b>Otimização de Deploy:</b> Implementação do comando aws s3 sync no lugar do cp, garantindo que apenas os arquivos alterados sejam transferidos, economizando tempo e recursos de rede.


## 🛠️ Implementação Prática
> 1. Conectar-se a uma instância do Amazon Linux EC2 usando SSM 
> 2. Configurar a AWS CLI 
> 3. Criar um bucket do S3 usando a AWS CLI
> 4. Criar um usuário do IAM que tenha acesso total ao Amazon S3 
> 5. Ajustar permissões de bucket do S3
> 6. Extrair os arquivos necessários para este laboratório 
> 7. Fazer upload de arquivos para o Amazon S3 usando a AWS CLI
> 8. Criar um arquivo em lote para tornar a atualização do site repetível


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-amazons3-awscli-activity-7441856084312498176-L_5d?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFVjvH5FfMZ9w/feedshare-image-high-res/B4DZ0bIq4mHMAU-/0/1774276751390?e=1785974400&v=beta&t=sxMBqg9QMzaxx9_41y49KailXmk9gL2OE8gdc7CjX1I" /> 

---

<img width="500" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHQC6Y84KCWBQ/feedshare-image-high-res/B4DZ0bIq5bIwAU-/0/1774276751446?e=1785974400&v=beta&t=zR4RU9h7Cz8BMGVlU2uAxFk7rtG_9yLmYopvxM5JK8M" /> 

---

<img width="500" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQE8d72h4PqJtw/feedshare-image-high-res/B4DZ0bIq9cIoAY-/0/1774276751824?e=1785974400&v=beta&t=Zs9HdgWQ7ijHWmRVi9nJycpXrqVffYAtoo5kr_vPbQU" /> 



## 🏁 Conclusão
A conclusão deste laboratório consolida competências essenciais em SysOps e automação de infraestrutura. A transição bem-sucedida da administração via interface gráfica para a operação baseada em scripts demonstra o domínio sobre o ciclo de vida de recursos de nuvem.

A validação do site em produção e a capacidade de atualizar o layout da aplicação em tempo real através do arquivo em lote comprovam a eficiência da arquitetura. Além disso, a implementação do comando aws s3 sync no desafio opcional coroa o projeto com uma mentalidade voltada para a otimização de performance e recursos, preparando a base para a integração de deploys de infraestrutura em esteiras automatizadas de CI/CD.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>