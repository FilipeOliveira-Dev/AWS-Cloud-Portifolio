# 🖥️ Projeto 06 - AWS Systems Manager


## 🌐 Visão Geral
Este laboratório prático do projeto 06 aborda a substituição de métodos tradicionais de administração de servidores pelo gerenciamento moderno de frotas utilizando o  **[AWS Systems Manager (SSM)](https://aws.amazon.com/pt/cli/?nc2=type_a)**.<br>
Em infraestruturas de nuvem em larga escala, depender de acessos via SSH individual, gerenciamento manual de pares de chaves criptográficas e abertura de portas de entrada (como a porta 22) gera gargalos operacionais e sérias vulnerabilidades de segurança. <br>
A atividade foca na centralização de dados operacionais e na automação de tarefas críticas de configuração, conformidade e governança. O uso do SSM elimina a necessidade de exposição direta das instâncias à internet, garantindo que a administração de frotas de servidores seja auditável, segura e altamente escalável.


## ⚙️ Arquitetura do Projeto
A implementação da arquitetura de gerenciamento centralizado foi estruturada através dos seguintes componentes do AWS Systems Manager:
- Auditoria e Descoberta (Fleet Manager & Inventory)
- Orquestração e Automação (Run Command).
- Gerenciamento de Configuração Dinâmica (Parameter Store).
- Acesso Remoto Seguro (Session Manager).


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEHGYuL5A1Lzw/feedshare-image-high-res/B4DZ0LdrvzKoAU-/0/1774013824634?e=1785974400&v=beta&t=ZtkKPUV-icF0pwbyGjFvJk8dSMvXNLBJpK2d4ClxiHo" />

---

<img width="600" height="250" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQH2sE2DoSGgOg/feedshare-image-high-res/B4DZ0Ldrw_HEAU-/0/1774013824549?e=1785974400&v=beta&t=J5nVNi5O70KPyNYdtknibRrzG6oKEBeP1nkYr96_QSg" />


## 📝 Tópicos Abordados

- Verificar configurações e permissões.
- Executar tarefas em vários servidores.
- Atualizar as configurações da aplicação.
- Acessar a linha de comando em uma instância.


## 🛠️ Implementação Prática
> 1. <b>Fleet Manager & Inventory:</b> Configurei a coleta automática de metadados e inventário de software das instâncias, permitindo auditorias rápidas sem acesso remoto direto.
> 2. <b>Run Command:</b> Realizei o deploy automatizado de uma aplicação web (Apache + PHP) em instâncias gerenciadas. O Run Command permite executar scripts em massa de forma auditável e segura.
> 3. <b>Parameter Store:</b> Implementei o gerenciamento de configurações "ao vivo". Usei parâmetros hierárquicos para ativar funcionalidades (Beta Features) na aplicação sem a necessidade de novos deploys de código.
> 4. <b>Session Manager:</b> Acessei a linha de comando das instâncias diretamente pelo navegador. Esta é uma alternativa muito mais segura ao SSH, pois elimina a necessidade de abrir portas de entrada (como a 22) e gerenciar chaves.


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-systemsmanager-ssm-activity-7440753290046447616-QwAb?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHaMLghA-DQBA/feedshare-image-high-res/B4DZ0LdrvHIAAU-/0/1774013824500?e=1785974400&v=beta&t=he7maCX-CFTfGpc5gmgYs5j1xz6ufSai-mWos5nGomM" /> 

---

<img width="600" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEJ2EAxXswZmQ/feedshare-image-high-res/B4DZ0LdrvYGsAg-/0/1774013824563?e=1785974400&v=beta&t=jE4_6_Ci47vxh45kvb7lD0tXWLG3T_8n4VfG3PwhQ7k" /> 

---

<img width="500" height="220" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQE2vQe9qPvSnA/feedshare-image-high-res/B4DZ0Ldrr9JoAU-/0/1774013824146?e=1785974400&v=beta&t=3N_vOeLqJ_iyizKwGK33TBKIaRCDy8aTdevhaQ-Tdu4" /> 



## 🏁 Conclusão
A conclusão deste projeto consolida o domínio sobre um dos pilares mais importantes da cultura DevOps e de Engenharia de Cloud: a segurança por design e automação de operações (SysOps/DevOps).
Ao integrar os recursos do AWS Systems Manager, o ambiente de infraestrutura atingiu um nível elevado de maturidade operacional.<br>
A eliminação do protocolo SSH em favor do Session Manager, combinada com deploys auditáveis via Run Command e parametrização dinâmica pelo Parameter Store, prova que é possível escalar o gerenciamento de centenas de servidores mantendo um controle rígido de segurança e conformidade. Essa experiência reflete diretamente os padrões de governança exigidos em arquiteturas corporativas complexas na AWS.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>