# 🖥️ Projeto 17 - Gerenciando o armazenamento

## 🌐 Visão Geral

Neste laboratório prático, nós exploramos diferentes estratégias para gerenciar e proteger dados na AWS utilizando a **[AWS Command Line Interface (AWS CLI)](https://aws.amazon.com/pt/ebs/)**. Nós utilizamos uma infraestrutura pré-configurada em uma VPC com a instância "Command Host" para administrar nossos recursos e gerenciar a instância "Processor". 

Ao longo das atividades, nós automatizamos o ciclo de vida de snapshots de volumes do **[Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/pt/ebs/)** por meio de scripts Python e programadores de tarefas, garantindo a retenção adequada de backups. Além disso, nós enfrentamos o desafio de otimizar a redundância de dados ao sincronizar o conteúdo de um diretório EBS com um bucket do **[Amazon S3](https://aws.amazon.com/pt/pm/serv-s3/)**Amazon S3, utilizando recursos de versionamento para garantir a recuperação de arquivos em cenários de exclusão acidental.



## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHiKmkIoMylEw/feedshare-image-high-res/B4DZ1Us2fQKIAc-/0/1775242537836?e=1791417600&v=beta&t=Pmn73WoKMwTaY2Jd2W-HcVuhCFLcVHjJucDeZj8hRc0" />


## 📝 Tópicos Abordados

- <b>Ciclo de Vida de Snapshots:</b> Automatizei a criação de snapshots de volumes EBS utilizando Cron jobs e scripts Python customizados para manter apenas as versões mais recentes, otimizando custos e organização.
- <b>Sincronização de Dados (Cloud Sync):</b> Utilizei a AWS CLI para sincronizar diretórios locais diretamente com o Amazon S3, utilizando a flag --delete para manter a paridade exata entre o servidor e o storage de objetos.
- <b>Recuperação de Desastres com Versionamento:</b> Implementei o S3 Bucket Versioning para recuperar arquivos deletados acidentalmente, demonstrando como restaurar versões específicas através dos comandos list-object-versions e get-object.
- <b>Infraestrutura e Segurança:</b> Configurei permissões granulares via IAM Roles para permitir que instâncias EC2 interagissem de forma segura com buckets e volumes.


## 🛠️ Implementação Prática

> 1. <b>Criar e configurar recursos</b>
> - <i>Etapa 1: Criar um bucket do S3</i>
> - <i>Etapa 2: Anexar perfil de instância a Processor</i>
> 2. <b>Gerar snapshots da instância</b>
> - <i>Etapa 1: Conectar-se à instância do EC2 chamada Command Host</i>
> - <i>Etapa 2: Gerar um snapshot inicial</i>
> - <i>Etapa 3: Programar a criação de snapshots subsequentes</i>
> - <i>Etapa 4: Reter os últimos dois snapshots</i>
> 3. <b>Desafio: Sincronizar arquivos com o Amazon S3</b>
> - <i>Etapa 1: Baixar e descompactar arquivos de exemplo</i>
> - <i>Etapa 2: Sincronizar arquivos</i>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-amazonebs-amazons3-activity-7445906884852695040-5z0x?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQE0xM_E-N-7_g/feedshare-image-high-res/B4DZ1Us2dCIYAU-/0/1775242537796?e=1791417600&v=beta&t=-EGxI2APkAn7uDaLKi_EcjJJJq6HCPYQDKonNtuMkF8" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFONsIY1L42Eg/feedshare-image-high-res/B4DZ1Us2cmHIAY-/0/1775242537599?e=1791417600&v=beta&t=yoXro21DDQe2df9r2k84eJStzRupRf3qnVzNvzq_sgA" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFRWYXrNL-VCQ/feedshare-image-high-res/B4DZ1Us2c5IcAU-/0/1775242537709?e=1791417600&v=beta&t=eg20RDOT02yt9vdgf_YO8sd9gJVWaa-Ak7ksGJg7tcA" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e aprimoramos nossas competências em automação e proteção de dados na AWS. Nós automatizamos a criação e a retenção de snapshots em instâncias do Amazon EC2, assegurando rotinas eficientes de backup para volumes do EBS. 

Adicionalmente, nós aplicamos comandos da AWS CLI para sincronizar dados do EBS diretamente com um bucket do Amazon S3 e alavancamos o recursos de versionamento do S3, garantindo uma camada extra de resiliência e a capacidade de recuperar arquivos excluídos com facilidade.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>