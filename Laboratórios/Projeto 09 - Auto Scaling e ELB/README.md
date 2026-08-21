# 🖥️ Projeto 09 - Usar Auto Scaling e Elastic Load Balancer


## 🌐 Visão Geral
Neste laboratório, usamos a **[AWS CLI (Command Line Interface)](https://aws.amazon.com/pt/cli/)** para criar uma instância do **[Amazon EC2](https://aws.amazon.com/pt/pm/ec2/)** para hospedar um servidor da web e criar uma imagem de máquina da Amazon (AMI) por meio dessa instância. Depois, usamos essa AMI como base para iniciar um sistema que seja dimensionado automaticamente sob uma carga variável usando o Amazon EC2 Auto Scaling.

Também criamo um Elastic Load Balancer para distribuir a carga por instâncias do EC2 criadas em várias Zonas de Disponibilidade pela configuração do Auto Scaling. 



## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGgif2G28EvPQ/feedshare-image-high-res/B4DZzvTzaxIkAU-/0/1773541472418?e=1788393600&v=beta&t=JNtd53LBxCcVr9yyVvCmLHUu-4VHJE44FJAlS5maNDs" />


## 📝 Tópicos Abordados

- <b>Criação de AMI personalizada:</b> Gerada a partir de uma instância EC2 para servir de base para o escalonamento.
- <b>Application Load Balancer (ALB):</b> Configurado para distribuir as requisições dos clientes de forma equilibrada.
- <b>Launch Template & Auto Scaling Group:</b> Definição de regras para provisionar novas instâncias automaticamente dentro de sub-redes privadas em resposta à demanda.
- <b>Monitoramento com CloudWatch:</b> Configuração de alarmes para observar a performance da infraestrutura e disparar ações de escalonamento.


## 🛠️ Implementação Prática
> 1. <b>Criar uma AMI para o Amazon EC2 Auto Scaling</b>
> - <i>Etapa 1: Conectar à instância Command Host</i>
> - <i>Etapa 2: Configurar a AWS CLI</i>
> - <i>Etapa 3: Criar uma instância do EC2</i>
> - <i>Etapa 4: Criar uma AMI personalizada</i>
> 2. <b>Criar um ambiente de Auto Scaling</b>
> - <i>Etapa 1: Criar um Application Load Balancer</i>
> - <i>Etapa 2: Criar um modelo de execução</i>
> - <i>Etapa 3: Criar um grupo do Auto Scaling</i>
> 3. <b>Verificar a configuração do Auto Scaling</b>
> 4. <b>Testar a configuração do Auto Scaling</b>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudcomputing-elasticloadbalancer-activity-7438772099760132096-B5pF?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGngDg9ebub3Q/feedshare-image-high-res/B4DZzvTzZaKQAU-/0/1773541472350?e=1788393600&v=beta&t=7ahcqRsuFHQ9QkmAS4ahjuc_T7zGZZrW9fQyQ-VwVBs" /> 

---

<img width="600" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQG0BQP208obHg/feedshare-image-high-res/B4DZzvTzZNGcAY-/0/1773541472367?e=1788393600&v=beta&t=0SVBO_mi1MV0PHoq8WUk-g0tW2yUCQPfkkQshmqjp1w" /> 

---

<img width="600" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHyZSudAZeVAQ/feedshare-image-high-res/B4DZzvTzZZGsAU-/0/1773541472426?e=1788393600&v=beta&t=bkvSO0nD0TysjotgcX9womcS5AeckOYrvgHfzBlyeNQ" /> 



## 🏁 Conclusão
A conclusão deste laboratório, nos mostrou conceitos fundamentais de infraestrutura como código (IaC) e arquitetura resiliente na AWS. Ao utilizar a AWS CLI, automatizamos a criação e o provisionamento de recursos, eliminando dependências da interface gráfica e garantindo maior precisão na implantação.

A construção da AMI personalizada a partir de uma instância EC2 base permitiu padronizar o ambiente do servidor web. Essa imagem serviu como modelo exato para que o Amazon EC2 Auto Scaling pudesse provisionar novas instâncias de forma homogênea e rápida, respondendo automaticamente a variações de tráfego e otimizando custos.

Por fim, a integração com o Application Load Balancer (ALB) garantiu alta disponibilidade e tolerância a falhas, distribuindo o tráfego de maneira eficiente entre múltiplas Zonas de Disponibilidade. O ambiente resultante é uma solução escalável, autorregenerável e pronta para suportar demandas variáveis de produção com alta performance.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>