# 🖥️ Projeto 03 - Introdução ao AWS IAM

## 🌐 Visão Geral
Este é o projeto do Laboratório 03, de introdução ao **[AWS Identity and Access Management (IAM)](https://aws.amazon.com/pt/iam/)**, o serviço fundamental para o gerenciamento de identidades e controle de acesso na nuvem da AWS. <br>
O objetivo principal foi compreender como mitigar riscos de segurança através da correta autenticação e autorização de identidades. Durante a prática, explorei a criação de políticas de senhas corporativas, a estrutura de usuários e grupos, e como as políticas de permissão (JSON) controlam o que cada usuário pode ou não fazer dentro do ambiente de nuvem.


## ⚙️ Arquitetura do Projeto
A arquitetura deste laboratório baseia-se no **[Princípio do Privilégio Mínimo (least privilege)](https://docs.aws.amazon.com/pt_br/wellarchitected/latest/framework/sec_permissions_least_privileges.html)**, garantindo que cada identidade possua apenas o acesso estritamente necessário para desempenhar suas funções.<br>
A estrutura foi organizada da seguinte forma:
- Políticas Globais: Implementação de uma política de senhas robusta para proteger a conta contra acessos de força bruta.
- Grupos e Permissões: Inspeção e uso de grupos de suporte e administração previamente configurados com permissões específicas para o Amazon S3 e Amazon EC2.
- Associação de Identidades: Distribuição estratégica de três usuários distintos (user-1, user-2 e user-3) em seus respectivos grupos funcionais.
- Validação de Acesso: Teste prático do comportamento das políticas de segurança através do URL de login personalizado do IAM, validando restrições de leitura, escrita e negações de acesso.

## 👤 Usuários e Grupos
| Usuário | Grupo | Permissões |
|---|---|---|
| user-1 | S3-Support | Acesso somente leitura ao Amazon S3 |
| user-2 | EC2-Support | Acesso somente leitura ao Amazon EC2 |
| user-3 | EC2-Admin | Visualizar, iniciar e interromper instâncias do EC2 |

<br>

<img width="600" height="250" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEy_48-aOVI6A/feedshare-image-high-res/B4DZzYqwHvH4AU-/0/1773161612162?e=1784764800&v=beta&t=TipEQa7-yDXzem-_-8lMSv8WPIBYyHykl3sFoS2FMAo" />


## 📝 Tópicos Abordados

- Políticas de Senha: Criação e aplicação de regras para fortalecer a segurança das contas.
- Gestão de Identidades: Exploração de usuários e grupos de usuários pré-configurados.
- Inspeção de Políticas: Análise detalhada de como as permissões são aplicadas a grupos específicos.
- Controle de Acessos: Atribuição de usuários a grupos com capacidades específicas ativas.
- Testes de Governança: Experimentos práticos para validar o efeito das políticas no acesso aos serviços.


## 🛠️ Implementação Prática
### 1. Criar uma política de senhas para a conta
### 2. Explorar usuários e grupos de usuários
### 3. Adicionar usuários a grupos
- Etapa 1: Adicionar user-1 ao grupo S3-Support.
- Etapa 2: Adicionar user-2 ao grupo EC2-Support
- Etapa 3: Adicionar user-3 ao grupo EC2-Admin
### 4. Fazer login e testar usuários



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudcomputing-iam-activity-7437178851392389120-k_tn?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="250" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGE7ytqEPJbGg/feedshare-image-high-res/B4DZzYqwI2KIAU-/0/1773161612817?e=1784764800&v=beta&t=IPQAz59dliBDXHgCf4kPwdAGHkpFlmaXS5praZzcY7s" /> 

--- 

<img width="600" height="250" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHW93_cQc2gxw/feedshare-image-high-res/B4DZzYqwIAKoAU-/0/1773161612822?e=1784764800&v=beta&t=339flzbolzyAgFGZoV6gmkYfrejOYGfXOuMNZSZztIk" />


## 🏁 Conclusão
A conclusão deste laboratório consolidou a importância vital da governança de acessos em ambientes de computação em nuvem. Ao aplicar na prática a política de senhas, gerenciar grupos funcionais e associar usuários a permissões específicas do S3 e EC2, ficou evidente como o AWS IAM previne erros operacionais e vazamentos de dados causados por acessos não autorizados.<br>
Testar os efeitos reais das políticas via URL de login do IAM permitiu validar a eficácia dos privilégios atribuídos, garantindo que a infraestrutura permaneça segura, auditável e alinhada às melhores práticas de segurança da informação.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>