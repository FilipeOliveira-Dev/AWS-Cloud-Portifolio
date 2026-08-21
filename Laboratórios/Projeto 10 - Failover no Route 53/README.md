# 🖥️ Projeto 10 - Roteamento de failover do Amazon Route 53

## 🌐 Visão Geral
Este laboratório prático tem como objetivo implementar uma política de roteamento com failover automático e alta disponibilidade utilizando o **[Amazon Route 53](https://aws.amazon.com/pt/route53/)** para uma aplicação web baseada na pilha LAMP.

A arquitetura distribui a carga de servidores web em instâncias Amazon EC2 provisionadas em diferentes Zonas de Disponibilidade (Multi-AZ) dentro da mesma região. Por meio da configuração de verificações de integridade (health checks) no Route 53, o DNS monitora continuamente o endpoint HTTP da instância primária.

Em caso de instabilidade ou falha no servidor principal, o Route 53 desvia o tráfego automaticamente para a instância secundária redundante e aciona notificações de alerta por e-mail, minimizando o tempo de inatividade (downtime) e garantindo a resiliência do serviço sem intervenção manual.



## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGC2wqxYvfUGg/feedshare-image-high-res/B4DZz9VpGgKgAU-/0/1773776835711?e=1788998400&v=beta&t=cu0PD50gj28nlof6hxexns1B0JS5nne25NQtwyQHKtk" />


## 📝 Tópicos Abordados

- <b>Health Checks Inteligentes:</b> Configurei verificações de saúde via HTTP que monitoram a integridade do endpoint primário em tempo real.
- <b>Alertas Automatizados:</b> Implementei alarmes via Amazon SNS para receber notificações imediatas por e-mail caso a instância principal apresente instabilidade.
- <b>Políticas de Roteamento de Failover:</b> Configurei registros de DNS do tipo A para instâncias primária e secundária, estabelecendo uma hierarquia de redundância.
- <b>Simulação de Desastre e Recuperação:</b> Testei a resiliência do sistema interrompendo a instância principal e validando o redirecionamento automático do tráfego para a região secundária em questão de minutos.


## 🛠️ Implementação Prática
> 1. <b>Confirmar os sites da cafeteria</b>
> 2. <b>Configurar uma health check do Route 53</b>
> 3. <b>Configurar registros do Route 53</b>
> - <i>Etapa 1: Criar um registro A para o site principal</i>
> - <i>Etapa 2: Criar um registro A para o site secundário</i>
> 4. <b>Verificar a resolução de DNS</b>
> 5. <b>Verificar a funcionalidade do failover</b>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-route53-cloudcomputing-activity-7439759290665697280-x4EX?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEQ22B7013Asw/feedshare-image-high-res/B4DZz9VpFfIwAY-/0/1773776835916?e=1788998400&v=beta&t=Rg0jFWyyJLIEXjlsFzv5HJH7tbN9W3p_FjWxANZPHNY" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHG9NVFBQGPsQ/feedshare-image-high-res/B4DZz9VpbhG0AU-/0/1773776837568?e=1788998400&v=beta&t=yA0z73M0Dn45Jw1IsK9ssVuvlMobep_irondFeaguec" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGDgvTHICju0w/feedshare-image-high-res/B4DZz9VpDFIkAU-/0/1773776835641?e=1788998400&v=beta&t=O9XvJ-ssmpR14UABPu9pvP2c85m_JqMQMKfAjcUYrlI" /> 



## 🏁 Conclusão
A conclusão deste laboratório consolida o entendimento sobre arquiteturas resilientes e tolerância a falhas na camada de rede da AWS.
Ao configurar o roteamento por failover e integrar as verificações de integridade do Route 53 aos mecanismos de notificação, estabelece-se um fluxo automatizado de recuperação de desastres (disaster recovery) em nível de DNS.

Essa implementação garante a continuidade operacional da aplicação web mesmo diante de indisponibilidades em uma Zona de Disponibilidade inteira, refletindo os padrões de alta disponibilidade exigidos em ambientes de produção corporativos.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>