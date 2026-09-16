# 🖥️ Projeto 23 - Automação com CloudFormation

## 🌐 Visão Geral

Neste laboratório prático, nós exploramos os conceitos de Infraestrutura como Código (IaC) para garantir a implantação consistente, automatizada e padronizada de recursos na AWS utilizando o AWS CloudFormation. Durante as atividades, nós iniciamos o processo criando e implantando uma pilha (stack) base contendo uma Nuvem Privada Virtual (VPC) e um grupo de segurança. 

Em seguida, nós consultamos a documentação técnica para evoluir o modelo do CloudFormation, declarando de forma declarativa um bucket do Amazon S3 e uma instância do Amazon EC2. Por fim, nós experimentamos todo o ciclo de vida da infraestrutura ao remover a pilha, garantindo que todos os recursos associados fossem encerrados de maneira limpa e automatizada.


## 📝 Tópicos Abordados

- <b>Provisionamento de VPC:</b> Criei uma rede virtual isolada, sub-redes e tabelas de rotas utilizando apenas código, garantindo que o ambiente seja 100% consistente em cada deploy.
- <b>Evolução de Infraestrutura:</b> Experimentei a agilidade de atualizar um "Stack" em execução. Adicionei um bucket Amazon S3 e uma instância EC2 ao ambiente apenas editando o arquivo de template e aplicando um update.
- <b>Parâmetros Inteligentes:</b> Implementei o uso do SSM Parameter Store para buscar automaticamente a AMI mais recente do Amazon Linux 2, tornando o código portátil entre diferentes regiões da AWS.
- <b>Ciclo de Vida Automatizado:</b> Pratiquei a limpeza total de recursos. Com um único comando de "Delete Stack", a AWS removeu automaticamente todos os recursos criados, evitando custos desnecessários e recursos órfãos.


## 🛠️ Implementação Prática

> 1. <b>Implantar uma pilha do CloudFormation</b>
> 2. <b>Adicionar um bucket do Amazon S3 à pilha</b>
> 3. <b>Adicionar uma instância do Amazon EC2 à pilha</b>
> 4. <b>Excluir a pilha</b>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudformation-iac-activity-7452715156939128832-IsRy?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQF-Jg_8SqXlVg/feedshare-image-high-res/B4DZ21c8A9G4Ag-/0/1776865756126?e=1791417600&v=beta&t=sXuwrHGX8-wugFB-8jRvOVBAzWRcAvpfPPY_a8qnEJw" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHahE_qK5j_Ng/feedshare-image-high-res/B4DZ21c8K9K4AU-/0/1776865756505?e=1791417600&v=beta&t=rWdJlJbsGgJaxDCDoDXERORY2_AoXzFBkpUrOjRblr0" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFtAF7dHuI9zQ/feedshare-image-high-res/B4DZ21c8MKHUAU-/0/1776865756579?e=1791417600&v=beta&t=kXxyWtLvDn3piUpQnVsf_XoCV-ODVQzou-nTUeQjnjk" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e dominamos os princípios fundamentais do AWS CloudFormation para orquestração de infraestrutura. Nós implantamos e editamos com sucesso pilhas do CloudFormation para criar uma VPC, configurar regras de segurança e provisionar recursos computacionais e de armazenamento, como instâncias EC2 e buckets do S3. 

Além disso, nós validamos a facilidade de gerenciamento e desmonte da infraestrutura ao excluir a pilha, eliminando riscos de desvio de configuração (drift) e custos desnecessários com recursos remanescentes.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>