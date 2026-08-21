# 🖥️ Projeto 14 - Configurar uma VPC

## 🌐 Visão Geral

Este laboratório prático aborda o provisionamento e a estruturação de uma rede isolada na AWS utilizando o **[Amazon VPC (Virtual Private Cloud)](https://aws.amazon.com/pt/vpc/)**.

O objetivo é criar uma arquitetura de rede segura dividida em sub-redes públicas e privadas. A sub-rede pública recebe um Internet Gateway (IGW) para tráfego bidirecional e hospeda um servidor Bastion Host, enquanto a sub-rede privada utiliza um NAT Gateway para permitir saída segura para a internet (para atualizações e patches) sem expor as instâncias a acessos externos diretos.

A atividade foca no controle de rotas, endereçamento IP e conectividade segura para instâncias Amazon EC2.


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEhaazoaSvRJw/feedshare-image-high-res/B4DZ0gJxtyKoAU-/0/1774360928303?e=1788998400&v=beta&t=2G5zTPhyauyvD6D9z6Acmk4Xg1mEwVvjpB02ZLY6_wU" />


## 📝 Tópicos Abordados

- <b>Segmentação de Rede (VPC & Subnets):</b> Criei uma VPC (10.0.0.0/16) com segmentação estratégica entre uma Public Subnet (para recursos com face externa) e uma Private Subnet (10.0.2.0/23) para proteger dados sensíveis.
- <b>Conectividade e Roteamento:</b> Implementei um Internet Gateway (IGW) para saída de internet na rede pública e um NAT Gateway para permitir que os recursos na rede privada baixem atualizações sem ficarem expostos diretamente à web.
- <b>Acesso Seguro (Bastion Server):</b> Configurei um servidor de salto (Bastion Host) na sub-rede pública, permitindo o acesso administrativo seguro às instâncias da sub-rede privada via SSH.
- <b>Deploy de Banco de Dados (MariaDB):</b> Utilizei o gerenciador de pacotes dnf para instalar o servidor MariaDB 10.5 em uma instância Amazon Linux 2023. Configurei o serviço para inicialização automática e validei a conectividade via CLI.
- <b>Governança de Tabelas de Rotas:</b> Personalizei as tabelas de rotas para direcionar o tráfego 0.0.0.0/0 corretamente, garantindo que o fluxo de dados seguisse rigorosamente as políticas de segurança.


## 🛠️ Implementação Prática

> 1. <b>Criar uma VPC e sub-redes</b>
> - <i>Etapa 1: Criar uma sub-rede pública e uma privada</i>
> 2. <b>Criar um gateway de internet</b>
> 3. <b>Configurar tabelas de rota</b>
> 4. <b>Iniciar um servidor bastion na sub-rede pública</b>
> 5. <b>Criar um gateway NAT</b>

> <b>Desafio opcional: Testar a sub-rede privada</b>
> - <i>Etapa 1: Iniciar uma instância na sub-rede privada</i>
> - <i>Etapa 2: Fazer login no servidor bastion</i>
> - <i>Etapa 3: Fazer login na instância privada</i>
> - <i>Etapa 4: Testar o gateway NAT</i>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudcomputing-vpc-activity-7442209147791613952-e06l?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEfC9ccF_NruA/feedshare-image-high-res/B4DZ0gJxzsGUAY-/0/1774360928527?e=1788998400&v=beta&t=ZqLo2r3gmjht7x-BvyXsJuZjUIvXfPrmykHhX3krxu4" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGZ1qvYWb0nyA/feedshare-image-high-res/B4DZ0gJxupJoAU-/0/1774360928993?e=1788998400&v=beta&t=etRJVvD4h0MczibtxVEbjkrZeBpQr_rBcQoibIvhkLY" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGwxpfNiOkEVg/feedshare-image-high-res/B4DZ0gJxuvIYAU-/0/1774360928142?e=1788998400&v=beta&t=fxJ5g9HXOEX3wnxfza1icg96qCrSe1GjtmRJmOn63sc" /> 



## 🏁 Conclusão
A conclusão do laboratório consolida o domínio sobre os fundamentos de redes e segurança na AWS.

A separação de recursos entre sub-redes públicas e privadas, associada ao gerenciamento de tabelas de rotas, Internet Gateway e NAT Gateway, estabelece uma base sólida para arquiteturas de alta disponibilidade. O uso do Bastion Host para acessar instâncias na sub-rede privada valida a aplicação de padrões de segurança de mercado, garantindo isolamento de infraestrutura e controle de acesso rigoroso.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>