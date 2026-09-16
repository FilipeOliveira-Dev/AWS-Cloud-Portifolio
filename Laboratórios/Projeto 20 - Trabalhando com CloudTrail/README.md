# 🖥️ Projeto 20 - Trabalhando com CloudTrail

## 🌐 Visão Geral

Neste laboratório prático, nós assumimos o papel de Sofia para solucionar um incidente de segurança e auditoria no site da cafeteria Café. Nós configuramos uma trilha no AWS CloudTrail para rastrear e auditar todas as ações executadas na conta da AWS após a detecção de uma violação no servidor Café Web Server. 

Para investigar a invasão, nós analisamos os logs do CloudTrail utilizando múltiplos métodos, como ferramentas de linha de comando no Linux (grep e AWS CLI) e consultas SQL analíticas no Amazon Athena. Por fim, nós identificamos as credenciais e o endereço IP do hacker no desafio de investigação, remediando a vulnerabilidade ao revogar o acesso do invasor, corrigir as configurações dos grupos de segurança e reforçar as diretrizes de acesso SSH e da aplicação.


## 🎬 Cenário do Laboratório

<img width="600" height="250" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHFrUhW-fuFKA/feedshare-image-high-res/B4DZ2Hq7vgJ4AU-/0/1776097672550?e=1791417600&v=beta&t=jwWsiNBCQ5yjZcu7EBZMh7qMuAIn-NqaIDseTJEGGU8" />


## 📝 Tópicos Abordados

- <b>Auditoria com AWS CloudTrail:</b> Implementei uma trilha de auditoria completa para monitorar cada API call realizada na conta, garantindo visibilidade total das ações dos usuários.
- <b>Análise Forense de Logs:</b> Utilizei o terminal Linux e o utilitário grep para filtrar milhares de registros JSON em busca de IPs e chamadas suspeitas.
- <b>SQL Analytics com Amazon Athena:</b> Para escalar a investigação, transformei os logs brutos do S3 em tabelas relacionais e executei consultas SQL complexas para identificar o exato momento em que o grupo de segurança foi violado.
- <b>Resposta a Incidentes no OS:</b> Identifiquei e removi um usuário malicioso (chaos-user) que estava logado via SSH, encerrei processos suspeitos e endureci a segurança do sistema operacional desativando a autenticação por senha no sshd_config.
- <b>Remediação de IAM:</b> Identifiquei o culpado e removi permanentemente suas credenciais de acesso (IAM User), fechando as brechas de segurança na infraestrutura.


## 🛠️ Implementação Prática

> 1. <b>Modificar um grupo de segurança e observar o site</b>
> 2. <b>Criar um log do CloudTrail e observar o site invadido</b>
> - <i>Etapa 1: Criar um log do CloudTrail</i>
> - <i>Etapa 2: Observar o site violado</i>
> 3. <b>Analisar os logs do CloudTrail usando grep</b>
> - <i>Etapa 1: Conectar-se à instância do EC2 de host usando SSH</i>
> - <i>Etapa 2: Baixar e extrair os logs do CloudTrail</i>
> - <i>Etapa 3: Analisar os logs usando grep</i>
> - <i>Etapa 4: Analisar os logs usando os comandos CloudTrail da AWS CLI</i>
> 4. <b>Analisar os logs do CloudTrail usando Athena</b>
> - <i>Etapa 1: Criar a tabela do Athena</i>
> - <i>Etapa 2: Analisar logs usando o Athena</i>

> <b>DESAFIO:</b> Identificar o hacker</b>
> 5. <b>Analisar ainda mais a invasão e melhorar a segurança</b>
> - <i>Etapa 1: Verificar os usuários do sistema operacional</i>
> - <i>Etapa 2: Atualizar a segurança SSH</i>
> - <i>Etapa 3: Corrigir o site</i>
> - <i>Etapa 4: Excluir o usuário hacker da AWS</i>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudsecurity-cloudtrail-activity-7449493585642749952-xP1N?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQE6R1XNBQc6dw/feedshare-image-high-res/B4DZ2Hq7zmJ4AU-/0/1776097673096?e=1791417600&v=beta&t=Hn1Nkj8zy06iUxJbzjdE2KYiSrqEQphHGe9tPbesqvI" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFvDSeg00WHWw/feedshare-image-high-res/B4DZ2Hq77OK0AU-/0/1776097673490?e=1791417600&v=beta&t=PEXj6uimM-DgMMapL9PFgLTjqYM21jvjUaYRwQbl4oU" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGAapX5awekOQ/feedshare-image-high-res/B4DZ2Hq7yfJgAU-/0/1776097673122?e=1791417600&v=beta&t=8IEbZ5cRaACENZPuaBx20xopWHDrHO0xP5fbVaCM21M" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e fortalecemos nossas habilidades em governança, auditoria e resposta a incidentes na nuvem da AWS. Nós implementamos com sucesso uma trilha no AWS CloudTrail e estruturamos uma rotina de análise de logs de auditoria combinando o utilitário grep, a AWS CLI e o Amazon Athena. 

Além disso, nós identificamos a origem do ataque, determinando o usuário, IP e método utilizado na violação do grupo de segurança, e aplicamos as devidas ações de mitigação ao remover os acessos não autorizados, restaurar a integridade do site e elevar o nível de proteção da infraestrutura no EC2.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>