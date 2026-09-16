# 🖥️ Projeto 21 - Gerenciameto de Recursos com Marcação

## 🌐 Visão Geral

Neste laboratório prático, nós abordamos a automação e o gerenciamento de governança na nuvem utilizando o gerenciamento de recursos por meio de marcação (tags). Nós nos conectamos à instância Command Host para inspecionar, filtrar e alterar tags em diversas instâncias Amazon EC2 utilizando a AWS CLI e expressões JMESPath com a opção --query. 

Ao longo das atividades, nós executamos scripts pré-configurados para automatizar o ciclo de vida dos recursos, interrompendo e iniciando instâncias em lote com base em atributos como ambiente e projeto. Por fim, nós enfrentamos o desafio de implementar a auditoria e o encerramento automático (terminate) de instâncias que não estivessem em conformidade com as políticas de marcação da organização.


## 📝 Tópicos Abordados

- <b>Consultas Avançadas com JMESPath:</b> Utilizei a AWS CLI com filtros complexos e queries --query para extrair dados específicos de instâncias baseadas em tags de Projeto, Versão e Ambiente.
- <b>Automação de Ciclo de Vida (Stopinator):</b> Implementei scripts (Bash e PHP SDK) para desligar e reiniciar ambientes de desenvolvimento inteiros de forma automática, uma prática essencial para otimização de custos (FinOps).
- <b>Política "Tag-or-Terminate":</b> Superei um desafio de segurança criando um processo automatizado que identifica e encerra instâncias não conformes (sem as tags obrigatórias), garantindo que nenhum recurso "fantasma" ou inseguro permaneça na infraestrutura.


## 🛠️ Implementação Prática

> 1. <b>Usar tags para gerenciar recursos</b>
> - <i>Etapa 1: Conectar-se à Command Host</i>
> - <i>Etapa 2: Alterar a tag Versão para o processo de desenvolvimento</i>
> 2. <b>Interromper e iniciar recursos por uma tag</b>
> - <i>Etapa 1: Examinar o script Stopinator</i>
> - <i>Etapa 2: Interromper e reiniciar o processo de desenvolvimento do ERPProject</i>
> 3. <b>Desafio: Terminar instâncias que não estejam em conformidade</b>
> - <i>Etapa 1: Revisar o script de Tag-Or-Terminate</i>
> - <i>Etapa 2: Execute o script</i>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudcomputing-awscli-activity-7449880777821057024-Uk5X?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFhnUKuMYmyXw/feedshare-image-high-res/B4DZ2NLFU3I4AU-/0/1776189987344?e=1791417600&v=beta&t=QVg6LWSiuyFYjBP49S5AAhyMVFD8fdneFlRg4SciAtI" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEO__DKbrYucQ/feedshare-image-high-res/B4DZ2NLFR8I8AU-/0/1776189987073?e=1791417600&v=beta&t=42BkysRKTGR0ORCEVLAgKBnfJsG4IfKu8Nl4k7OERjo" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGAj5G6_Ta6vg/feedshare-image-high-res/B4DZ2NLFKqI4AY-/0/1776189986507?e=1791417600&v=beta&t=GZsuPghXCL_5mq2wTjC5CKP3ccetnScdByvauMOY_m4" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e consolidamos práticas essenciais de automação, governança e redução de custos na AWS. Nós aplicamos e atualizamos tags em recursos existentes do Amazon EC2 e dominamos o uso da AWS CLI para localizar instâncias específicas por meio de filtros de marcação. 

Além disso, nós utilizamos scripts para gerenciar o estado das instâncias com base em suas tags e validamos a execução de rotinas de conformidade para encerrar automaticamente recursos fora dos padrões definidos.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>