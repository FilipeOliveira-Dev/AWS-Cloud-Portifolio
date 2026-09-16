# 🖥️ Projeto 22 - Otmizando a Utilização

## 🌐 Visão Geral

Neste laboratório prático, nós exploramos estratégias de otimização de recursos e redução de custos operacionais na AWS para o aplicativo web da cafeteria Café. Assumindo o papel de Sofia, nós nos conectamos via SSH às instâncias para desinstalar o banco de dados MariaDB local que já não era necessário devido à migração para o Amazon RDS, liberando armazenamento no servidor. 

Em seguida, nós redimensionamos a instância Amazon EC2 para um tipo menor e mais adequado à nova demanda (T3 micro). Para validar o impacto financeiro dessa readequação, nós utilizamos a Calculadora de Preços da AWS para estimar e comparar os custos antes e depois das modificações, projetando a economia gerada para o negócio.



## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHdle8zeapARw/feedshare-image-high-res/B4DZ2SBh0zJ0AU-/0/1776271367974?e=1791417600&v=beta&t=0tpPCjy5Hn4s82ZBrA4Xs6RCgnQ-Zq6CEBlu_O_lYj4" />


## 📝 Tópicos Abordados

- <b>Remoção de Resquícios (Decommissioning):</b> Realizei a desinstalação completa do MariaDB na instância EC2 via terminal, liberando espaço em disco e ciclos de CPU desnecessários.
- <b>Right Sizing com AWS CLI:</b> Utilizei a linha de comando para interromper a instância e modificar seu atributo de tipo de t3.small para t3.micro, adequando o poder computacional à nova realidade da aplicação.
- <b>FinOps e Estimativa de Custos:</b> Utilize a AWS Pricing Calculator para realizar uma análise comparativa de custos. A otimização gerou uma economia projetada de aproximadamente 13% no faturamento mensal dos serviços!
 > AWS Services Before Optimization Estimated Monthly Cost: $74.04

 > AWS Services After Optimization Estimated Monthly Cost: $64.45
- <b>Validação de Continuidade:</b> Garanti que, mesmo após o downsizing e a troca de IPs/DNS, a aplicação permanecesse 100% funcional e integrada ao banco de dados gerenciado.


## 🛠️ Implementação Prática

> 1. <b>Otimizar o site para reduzir custos</b>
> - <i>Etapa 1: Conectar-se à instância da cafeteria Café usando SSH</i>
> - <i>Etapa 2: Conectar-se à instância de host da CLI usando SSH</i>
> - <i>Etapa 3: Desinstalar o MariaDB e redimensionar a instância</i>
> 2. <b>Usar a Calculadora de Preços da AWS para estimar os custos dos serviços da AWS</b>
> - <i>Etapa 1: Calcular os custos antes da otimização</i>
> - <i>Etapa 2: Calcular os custos após a otimização</i>
> - <i>Etapa 3: Estimar a economia de custos projetada para a cafeteria Café</i>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudcomputing-finops-activity-7450222121261387776-Ewui?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGUNN4iazJgAQ/feedshare-image-high-res/B4DZ2SBh0pGUAU-/0/1776271368228?e=1791417600&v=beta&t=_CjhVZPdoclTaYTmdtzjyNijhrkZ0YLlCz5Fcx55rpU" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFmoj9XnUXfHQ/feedshare-image-high-res/B4DZ2SBhycGUAc-/0/1776271367811?e=1791417600&v=beta&t=7oq4dRTs4Jkl59cTPv6-gh8fk2pHT0861lkm4skXtZc" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQESZkKOHZ5iBg/feedshare-image-high-res/B4DZ2SBh0rK0AU-/0/1776271368256?e=1791417600&v=beta&t=QvWJVbLLKJ62kVXhxqXnasqh39_DhJHAEu5yD3avkt8" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e aplicamos na prática conceitos essenciais de otimização financeira e dimensionamento de recursos na nuvem. Nós reduzimos a pegada de armazenamento e processamento da aplicação ao remover o banco de dados local desativado e alterar a instância do Amazon EC2 para uma família mais econômica. 

Além disso, nós utilizamos a Calculadora de Preços da AWS para quantificar os custos e mensurar com precisão a economia obtida, alinhando a arquitetura tecnológica às melhores práticas de gestão de custos da AWS.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>