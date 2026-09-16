# 🖥️ Projeto 24 - Amazon SageMaker

## 🌐 Visão Geral

Neste laboratório prático, nós avançamos na exploração do conjunto de dados de biomecânica da coluna vertebral, focando no desenvolvimento e treinamento de modelos de Machine Learning na nuvem. Nós iniciamos acessando e configurando um ambiente de desenvolvimento gerenciado através de uma instância de bloco de notas (notebook instance) no Amazon SageMaker. 

Ao longo do laboratório, nós dividimos o conjunto de dados original em três partições distintas — treinamento, validação e teste — para garantir um processo de avaliação preciso. Por fim, nós utilizamos o algoritmo supervisionado XGBoost para treinar o modelo na infraestrutura do SageMaker, preparando a base para previsões analíticas.


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQG8vyzrV3j88Q/feedshare-image-high-res/B4DZ3AJWP.JYAU-/0/1777045170010?e=1791417600&v=beta&t=_lsM8M5yyBxpZALgRTmrYENFuUTVDy9JcIB2qfeYFic" />


## 📝 Tópicos Abordados

- <b>Análise de Dados com JMESPath:</b> Pratiquei a filtragem de documentos JSON complexos usando expressões JMESPath para extrair informações específicas de recursos da pilha diretamente via linha de comando.
- <b>Depuração de UserData:</b> Diagnostiquei uma falha de "WaitCondition" acessando os logs da instância (cloud-init-output.log). Identifiquei um erro de sintaxe no script de inicialização (yum install) que impedia o servidor web de subir corretamente.
- <b>Detecção de Desvios (Drift Detection):</b> Simulei mudanças manuais na infraestrutura (configurações de segurança fora do código) e utilizei o CloudFormation para detectar esses desvios, reforçando a importância da imutabilidade da infraestrutura.


## 🛠️ Implementação Prática

> 1. <b>acessar uma instância do bloco de notas no Amazon SageMaker</b>
> 2. <b>abrir um bloco de anotações em sua instância do bloco de notas</b>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-cloudformation-iac-activity-7453467674149412864-gO4h?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHRYDhGYATTrg/feedshare-image-high-res/B4DZ3AJWQKG4AY-/0/1777045169936?e=1791417600&v=beta&t=uIjeuOrUFAkKsnpbsnTJ5Pzi1eRl5SLOKT5Ga4O4LAA" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGKwnS2jYQnUA/feedshare-image-high-res/B4DZ3AJWTWG4AU-/0/1777045170216?e=1791417600&v=beta&t=bo__dGHQA2qKbaSEQ-WdA8Wk47htXSH7hUVPGMzxiVM" /> 

---

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHlouX7v6k4vQ/feedshare-image-high-res/B4DZ3AJWNfJYAY-/0/1777045169742?e=1791417600&v=beta&t=gutrY0f-cY7NkrRr7cRzNbxxzyO0TvwkGLM2tHeUSOE" /> 



## 🏁 Conclusão

Nós concluímos este laboratório com êxito e consolidamos práticas fundamentais na preparação de dados e no treinamento de modelos com o Amazon SageMaker. Nós estruturamos corretamente a divisão dos dados biomecânicos em conjuntos de treinamento, validação e teste, garantindo a integridade do processo de aprendizado de máquina. 

Além disso, nós configuramos e executamos o treinamento do algoritmo XGBoost dentro da plataforma do SageMaker, adquirindo experiência prática nas etapas iniciais do ciclo de vida de Machine Learning na AWS.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>