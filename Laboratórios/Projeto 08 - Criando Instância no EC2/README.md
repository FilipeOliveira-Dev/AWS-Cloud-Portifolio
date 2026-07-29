# 🖥️ Projeto 08 - Criando Instância no EC2


## 🌐 Visão Geral
Este laboratório prático explora dois métodos fundamentais para a criação e gerenciamento de instâncias **[Amazon EC2](https://aws.amazon.com/pt/pm/ec2/)**: a interface visual via Console de Gerenciamento da AWS e a execução de comandos programáticos através da **[AWS CLI (Command Line Interface)](https://aws.amazon.com/pt/cli/)**.<br>
A arquitetura do projeto implementa o conceito de segurança com um Host Bastion (servidor de salto). A primeira instância é provisionada manualmente pelo console e acessada com segurança via EC2 Instance Connect (sem a necessidade de expor chaves SSH locais). A partir deste Bastion, assume-se o papel de administração via terminal para recuperar metadados de rede (Sub-redes e Security Groups) e disparar a criação automatizada do servidor web final utilizando a AWS CLI com inclusão de um script de User Data para bootstrap de aplicação.<br>
A atividade reforça o critério de escolha de ferramentas no dia a dia DevOps: o Console para testes pontuais e o uso de CLI/Scripts para automações repetíveis e confiáveis de infraestrutura.


## 🎬 Cenário do Laboratório

<img width="600" height="400" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQFrJyvvj70TCQ/feedshare-shrink_1280/B4DZ0lnyCvKoAM-/0/1774452679137?e=1787184000&v=beta&t=TKaC4vlGy0DADQNIdw3b1SsJYPIGqBFCiqi9By2DeHM" />


## 📝 Tópicos Abordados

- <b>Arquitetura de Acesso Seguro:</b> Iniciei um Bastion Host via Console de Gerenciamento, configurando um grupo de segurança restrito para permitir apenas conexões SSH controladas.
- <b>Conectividade Moderna:</b> Utilizei o EC2 Instance Connect para um acesso seguro e sem a necessidade de gerenciar chaves privadas locais.
- <b>Automação via AWS CLI:</b> Do terminal do Bastion Host, utilizei a linha de comando para recuperar dinamicamente a AMI mais recente, IDs de sub-rede e grupos de segurança para lançar um servidor web funcional.
- <b>Bootstrapping com User Data:</b> Implementei scripts de dados do usuário para automatizar a instalação do servidor Apache e o deploy da aplicação web no momento da inicialização da instância.


## 🛠️ Implementação Prática
> 1. <b>Iniciar uma instância do EC2 usando o Console de Gerenciamento da AWS</b>
> - <i>Etapa 1: Escolher um nome e tags</i>
> - <i>Etapa 2: Escolher uma AMI</i>
> - <i>Etapa 3: Escolher um tipo de instância</i>
> - <i>Etapa 4: Configurar um par de chaves</i>
> - <i>Etapa 5: Definir as configurações de rede</i>
> - <i>Etapa 6: Adicionar armazenamento</i>
> - <i>Etapa 7: Iniciar uma instância do EC2</i>
> 2. <b>Fazer login no host bastion</b>
> 3. <b>Iniciar uma instância do EC2 usando a AWS CLI</b>
> - <i>Etapa 1: Recuperar a AMI que será usada</i>
> - <i>Etapa 2: Recuperar a sub-rede que será usada </i>
> - <i>Etapa 3: Recuperar o grupo de segurança que será usado</i>
> - <i>Etapa 4: Baixar um script de dados do usuário</i>
> - <i>Etapa 5: Iniciar a instância e aguardar até que esteja funcionando</i>
> - <i>Etapa 6: Testar o servidor web</i>
> 4. <b>Desafio opcional 1: Conectar-se a uma instância do EC2</b>
> 5. <b>Desafio opcional 2: Corrigir a instalação do servidor web</b>



## 📸 Evidências

### **[Publicação no LinkedIn](https://www.linkedin.com/posts/filipeoliveiradasilva_aws-amazonec2-awscli-activity-7442593978665050112-7bYi?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAR6GdcBABiosNPcpPrXwA4Y9q4rI9ijMWI)**

<img width="600" height="350" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEj5BEeLcdpZg/feedshare-image-high-res/B4DZ0lnyElIEAY-/0/1774452679628?e=1787184000&v=beta&t=4dD7KsPUE8Yiqjh9pxCI5f4F2kSFbnp1yxOCmoCe3r4" /> 

---

<img width="500" height="200" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQHOtOzAxRQVeg/feedshare-image-high-res/B4DZ0lnyN0KgAU-/0/1774452679960?e=1787184000&v=beta&t=fVEr_LzsoOVDtuskHDWNC7Eo331iXns7BPW3qS9QMdQ" /> 

---

<img width="800" height="400" alt="image" src="https://media.licdn.com/dms/image/v2/D4D22AQEij7Nr3xbJrA/feedshare-image-high-res/B4DZ0lnyHFIAAY-/0/1774452679920?e=1787184000&v=beta&t=Vau-fVk0Q-5Kn9SHY8sg3_XAewvdCDtuzKN7MGAfCdM" /> 



## 🏁 Conclusão
A conclusão deste laboratório consolida o domínio sobre o provisionamento híbrido de computação na AWS, combinando controle manual estratégico e automação via linha de comando.<br>
A implementação do fluxo — desde o lançamento do Bastion via Console até o bootstrap do servidor web com dados de usuário via CLI — demonstra a compreensão sobre arquiteturas em camadas e redes isoladas. Além disso, a resolução dos desafios de conectividade e correção de pacotes do servidor web reforça habilidades essenciais de troubleshooting e administração de sistemas Linux em ambiente de nuvem, preparando a base para automações ainda mais robustas com ferramentas de Infraestrutura como Código.

---

<div align="center">

**Filipe Oliveira** · DevOps | AWS Cloud Practitioner | Estudante de Tecnologia da Informação ·

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/filipeoliveiradasilva/)
[![GitHub](https://img.shields.io/badge/GitHub-FF9900?style=flat&logo=github&logoColor=white)](https://github.com/FilipeOliveira-Dev)

</div>