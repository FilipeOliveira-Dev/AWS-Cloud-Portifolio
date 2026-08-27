# 🖥️ Projeto 15 - Solucionar Problemas na VPC

## 🌐 Visão Geral

Implementação de monitoramento de tráfego IP e resolução de falhas de conectividade em topologia multi-VPC no ambiente AWS. A ausência de visibilidade sobre os fluxos de rede estende o tempo médio de resolução (MTTR) de incidentes e expõe a infraestrutura a riscos de segurança. 

Para eliminar essa opacidade, a solução combina a centralização de VPC Flow Logs em um bucket Amazon S3 dedicado para auditoria técnica com a identificação e correção de bloqueios em Route Tables, Security Groups e Network ACLs, restabelecendo a comunicação entre instâncias Amazon EC2.


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEdrUTbs61EgA/feedshare-shrink_1280/B4DZ0_b8xiKMAM-/0/1774885785074?e=1789603200&v=beta&t=Fls2aqgGbw_CJYjqyxkiPbtYzFsUABojkxiyzYQavUc" />


## 📝 Tópicos Abordados

- <b>Monitoramento e Auditoria:</b> Implementei VPC Flow Logs destinados a um bucket do Amazon S3 para capturar e analisar todo o tráfego IP da rede.
- <b>Diagnóstico via CLI:</b> Utilizei exclusivamente a AWS CLI e utilitários como nmap para identificar portas bloqueadas e falhas de comunicação.
- <b>Resolução de Roteamento:</b> Identifiquei e corrigi tabelas de rotas mal configuradas, restabelecendo o fluxo de tráfego entre a sub-rede pública e o Internet Gateway.
- <b>Ajuste de ACLs de Rede (NACL):</b> Solucionei um bloqueio de acesso SSH de "nível 2", identificando regras restritivas em listas de controle de acesso de rede que impediam a administração das instâncias.
- <b>Análise Forense de Logs:</b> Utilize comandos Linux (grep, gunzip) para filtrar registros de REJECT nos logs de fluxo, correlacionando carimbos de data/hora Unix e endereços IP para validar as tentativas de acesso.


## 🛠️ Implementação Prática

> 1. <b>Conectar-se à instância CLI Host</b>
> - <i>Etapa 1: Configurar a AWS CLI na instância CLI Host</i>
> 2. <b>Criar logs de fluxo da VPC</b>
> 3. <b>Solucionar problemas de configuração da VPC para permitir acesso aos recursos.</b>

> <b>Desafio Opcional da solução de problemas:
> 1. <b>Analisar logs de fluxo</b>
> - <i>Etapa 1: Baixar e extrair os logs de fluxo</i>
> - <i>Etapa 2: Analisar os logs</i>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-vpc-flowlogs-activity-7444410558759645184-XheQ?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFVXlMQABjQ8w/feedshare-image-high-res/B4DZ0_b8voH4AU-/0/1774885785459?e=1789603200&v=beta&t=cZtkNrCaa7bHZHzDAdvtzNyp9EBtx_CCbs47cpMhqAY" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFdrl11ypGF-Q/feedshare-image-high-res/B4DZ0_b8w.JQAU-/0/1774885785269?e=1789603200&v=beta&t=1IYUYFOIrols0LNqmyPojoUO530QkQSDb04LwpUoM-4" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQF7QTa5n_9D6g/feedshare-image-high-res/B4DZ0_b8yoKoAU-/0/1774885785325?e=1789603200&v=beta&t=uOev5wwMpzmqLoVljB-FeP2o9jHLucP6uJuWxBNkoho" /> 



## 🏁 Conclusão
A estruturação de VPC Flow Logs integrada ao Amazon S3 consolida a telemetria necessária para auditoria de segurança e diagnóstico avançado de redes na AWS. 

A abordagem orientada a dados reduz o tempo de inatividade não planejado e eleva o nível de maturidade da infraestrutura, alinhando a operação aos pilares de Excelência Operacional e Segurança do AWS Well-Architected Framework.


---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>