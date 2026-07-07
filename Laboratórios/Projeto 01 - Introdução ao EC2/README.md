# 🖥️ Projeto 01 - Introdução ao Amazon EC2

## 🌐 Visão Geral
Este é o projeto do Laboratório 01, que apresenta uma visão geral básica de como executar, redimensionar, gerenciar e monitorar uma instância do **[Amazon EC2 (Elastic Compute Cloud)](https://aws.amazon.com/pt/pm/ec2/)** - um dos pilares da **[Amazon Web Services (AWS)](https://aws.amazon.com/)** - aplicando conceitos importantes da computação em nuvem relacionados à segurança, monitoramento e gerenciamento de recursos.

## ⚙️ Arquitetura do Projeto
A solução utiliza um servidor web baseado em EC2, protegido por um Security Group que libera apenas o tráfego HTTP. O provisionamento de armazenamento é feito via volumes EBS, e a infraestrutura é monitorada por soluções nativas da AWS. Para mitigar riscos operacionais, foi implementada a proteção contra exclusão acidental da instância.

## 📝 Tópicos Abordados
- Iniciar um servidor web com proteção contra encerramento (termination protection) ativada
- Monitorar sua instância do EC2
- Modificar o grupo de segurança (security group) que o servidor web está usando para permitir acesso HTTP
- Redimensionar sua instância do Amazon EC2 de acordo com a necessidade
- Testar a proteção contra encerramento
- Terminar a instância do EC2

## 🛠️ Implementação Prática
### 1. Iniciar sua instância do EC2
- Etapa 1: Nomear sua instância do EC2
- Etapa 2: Selecionar uma imagem de máquina da Amazon (AMI)
- Etapa 3: Selecionar um tipo de instância
- Etapa 4: Configurar um par de chaves
- Etapa 5: Definir as configurações de rede
- Etapa 6: Adicionar armazenamento
- Etapa 7: Configurar detalhes avançados
- Etapa 8: Iniciar uma instância do EC2
### 2. Monitorar a instância
### 3. Atualizar o grupo de segurança e acessar o servidor web
### 4. Redimensionar a instância: tipo de instância e volume do EBS
- Etapa 1: Interromper a instância
- Etapa 2: Alterar o tipo de instância
- Etapa 3: Redimensionar o volume do EBS.
- Etapa 4: Iniciar a instância redimensionada
### 5. Testar a proteção contra encerramento

## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudcomputing-amazonec2-activity-7435398636865343488-2b1S?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="800" height="600" alt="image" src="https://media.licdn.com/dms/image/v2/D4E22AQGbRc6gxmOrRQ/feedshare-image-high-res/B4EZy_XqB7JkBU-/0/1772737175954?e=1784764800&v=beta&t=5xkR3yvfoecrw1FIxfMj6cmeN3kj7MVRB3Zwux-nHdU" />

## 🏁 Conclusão
A realização deste laboratório consolidou, na prática, os conceitos de criação e administração de servidores em nuvem. O processo permitiu configurar um ambiente funcional com controle de acesso rigoroso, monitoramento de desempenho e mecanismos de segurança contra falhas operacionais.<br>
A experiência também evidenciou a flexibilidade e a escalabilidade da computação em nuvem, capacitando a realização de testes e ajustes dinâmicos para atender a diferentes demandas de infraestrutura de forma eficiente.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>