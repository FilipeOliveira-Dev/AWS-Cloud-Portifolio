# 🖥️ Projeto 05 - Instalando e Configurando o AWS CLI


## 🌐 Visão Geral
Este é o projeto do Laboratório 05, que aborda a instalação, configuração e operação da **[AWS CLI (Command Line Interface)](https://aws.amazon.com/pt/cli/?nc2=type_a)** em um ambiente Linux Red Hat Enterprise Linux (RHEL) provisionado na AWS.
Diferente de distribuições como o Amazon Linux, o RHEL não traz a interface de linha de comando da AWS pré-instalada, simulando um cenário real de migração ou configuração de servidores limpos (On-Premises ou Cloud).<br>
A atividade foca na eliminação da dependência da interface gráfica (Console de Gerenciamento), estabelecendo uma conexão segura via SSH para configurar chaves de acesso programáticas (Access Key ID e Secret Access Key) e gerenciar recursos de segurança e governança de forma automatizada e escalável.


## ⚙️ Arquitetura do Projeto
A implementação seguiu um fluxo lógico de administração de sistemas e gerenciamento de identidades, dividido nas seguintes etapas estruturais:
- Acesso e Conectividade: Estabelecimento de túnel seguro via protocolo SSH para comunicação direta com a instância EC2 baseada em Red Hat, isolada dentro de uma VPC (Virtual Private Cloud).
- Provisionamento do Ambiente: Download, instalação e validação do pacote oficial da AWS CLI diretamente no sistema operacional RHEL via terminal.
- Auditoria de Governança: Mapeamento e comparação das entidades do AWS IAM (Identity and Access Management). Configuração das credenciais programáticas na CLI (aws configure) para espelhar as permissões da conta e consulta de usuários, grupos e políticas via linha de comando.
- Desafio Técnico: Extração cirúrgica e exportação da política gerenciada pelo cliente (lab_policy). O processo envolveu a listagem de políticas com escopo local, a consulta à versão ativa do documento através da API do IAM e a canalização do payload limpo para um arquivo físico lab_policy.json utilizando operadores de redirecionamento de saída do Linux (>).


## 🎬 Cenário do Laboratório

<img width="600" height="300" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEYrPKehNftwQ/feedshare-image-high-res/B4DZ0BmjUDJQAY-/0/1773848377144?e=1785369600&v=beta&t=yKx-9Avz0Em6i4ElKxlxB4GO6LWmCkgjQ-68Mig_7l4" />


## 📝 Tópicos Abordados

- Ambiente Linux: Realizei a instalação manual do AWS CLI v2, garantindo que todas as dependências estivessem corretas em uma distribuição Red Hat.
- Configuração de Segurança: Conectei o CLI à minha conta AWS utilizando Access Keys e Secret Keys, definindo regiões e formatos de saída (JSON).
- Interação com IAM: Explorei e listei usuários e políticas de segurança diretamente pelo terminal, sem tocar no console web.
- Desafio de Políticas: Utilizei comandos avançados como list-policies e get-policy-version para extrair e salvar documentos de política IAM em formato JSON.


## 🛠️ Implementação Prática
> 1. <b>Conectar-se à instância do EC2 do Red Hat usando SSH</b>
> 2. <b>Instalar a AWS CLI em uma instância do Linux do Red Hat </b>
> 3. <b>Observar os detalhes de configuração do IAM no Console de Gerenciamento da AWS</b>
> 4. <b>Configurar a AWS CLI para conectar-se à conta da AWS</b>
> 5. <b>Observar os detalhes de configuração do IAM usando a AWS CLI</b>


## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-awscli-iam-activity-7440059351702327296-QQMj?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="400" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQGc7jrLgElK_g/feedshare-image-high-res/B4DZ0BmjOJIoAU-/0/1773848376548?e=1785369600&v=beta&t=y980hMsFm3HtF4u8hR8D6af00rbKMNXcLMqBDacVLHk" /> 

---

<img width="600" height="400" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHQ1h8Me1UF4Q/feedshare-image-high-res/B4DZ0BmjSnIkAY-/0/1773848377185?e=1785369600&v=beta&t=SAhI3Zmy71Q6smC8mdUdQ56tIpA5XIO3dY-0FCVJ4TY" /> 



## 🏁 Conclusão
A conclusão deste laboratório consolida uma das habilidades mais críticas para a cultura DevOps: a operação puramente via terminal e automação de comandos.
A capacidade de extrair artefatos de infraestrutura, como políticas do IAM em formato JSON sem interagir com o console visual, prepara a base para a criação de scripts de automação (Shell Scripting/Python) e auditorias de conformidade de segurança em larga escala. <br>
O sucesso no desafio prático comprova o domínio sobre a documentação oficial da AWS CLI e reforça o entendimento sobre autenticação programática e o ciclo de vida de políticas de segurança como código.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>