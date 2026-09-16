# 🖥️ Projeto 16 - Trabalhando com EBS

## 🌐 Visão Geral

Neste laboratório prático, foi explorado a utilização do **[Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/pt/ebs/)** como uma solução de armazenamento em bloco de alto desempenho para o **[Amazon Elastic Compute Cloud (Amazon EC2)](https://aws.amazon.com/pt/pm/ec2/)**.

Ao longo das tarefas, passamos por todo o ciclo de vida de um volume EBS: desde a criação, vinculação e formatação (criação de sistema de arquivos) em uma instância EC2, até o gerenciamento de persistência de dados. Além disso, aprendemos a garantir a alta disponibilidade e o backup dos dados por meio de snapshots, testando na prática a restauração e montagem de um novo volume a partir de um ponto de recuperação.



## 🎬 Cenário do Laboratório

<img width="600" height="250" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGWhQeWnMHF4Q/feedshare-image-high-res/B4DZ1EDGQVHwAU-/0/1774963172151?e=1791417600&v=beta&t=214HJu2BB-krIbz3TG-avbHhrBHulfciuNsM7cSnxB8" />


## 📝 Tópicos Abordados

- <b>Provisionamento e Montagem:</b> Criei volumes EBS gp2 e os anexei a instâncias EC2, configurando sistemas de arquivos ext3 e garantindo a persistência da montagem via /etc/fstab.
- <b>Estratégia de Backup (Snapshots):</b> Realizei backups point-in-time utilizando Snapshots armazenados de forma durável no Amazon S3.
- <b>Recuperação de Desastres:</b> Simulei a perda de dados e realizei a restauração completa criando um novo volume a partir de um snapshot, validando a integridade dos arquivos recuperados.
- <b>Administração via CLI:</b> Utilizei o terminal Linux para gerenciar pontos de montagem e diretórios de armazenamento (/mnt/data-store).


## 🛠️ Implementação Prática

> 1. <b>Criar um volume do EBS</b>
> 2. <b>Anexar o volume a uma instância do EC2</b>
> 3. <b>Conectar-se à instância do EC2 chamada Lab</b>
> 4. <b>Criar e configurar o sistema de arquivos</b>
> 5. <b>Criar um snapshot do Amazon EBS</b>
> 6. <b>Restaurar o snapshot do Amazon EBS</b>
> - <i>Etapa 1: Criar um volume usando o snapshot</i>
> - <i>Etapa 2: Anexar o volume restaurado à instância do EC2</i>
> - <i>Etapa 3: Montar o volume restaurado</i>




## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-amazonebs-cloudcomputing-activity-7444735151915450369-JCWT?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQF_i6m3oMSd2w/feedshare-image-high-res/B4DZ1EDGRoKoAU-/0/1774963156915?e=1791417600&v=beta&t=3mQ9QT13UZvQ1mf25GbIhzPDnlcZTuLOlPC07-LckMk" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEJnu1LGyLqFA/feedshare-image-high-res/B4DZ1EDGTsKAAU-/0/1774963160299?e=1791417600&v=beta&t=dMDCITMAkSRU5aV8RmtDczy8TKoO0zRQ0jBd3n4cQOQ" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGftZ4jBAvw_w/feedshare-image-high-res/B4DZ1EDGUyHMAU-/0/1774963157319?e=1791417600&v=beta&t=w1GcRME2h6QtC32r9ir0Y1JUmRR9ukig2g0fFbOa6GI" /> 



## 🏁 Conclusão
Concluímos este laboratório com êxito e adquirimos competências fundamentais para o gerenciamento de armazenamento na AWS. Ao criar, anexar, formatar e montar um volume EBS em uma instância EC2, nós experimentamos como fornecer armazenamento de bloco persistente para  nossas aplicações. Ademais, a prática de criação e restauração de snapshots do Amazon EBS demonstrou como proteger dados críticos e implementar estratégias eficientes de backup e recuperação de desastres na nuvem.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>