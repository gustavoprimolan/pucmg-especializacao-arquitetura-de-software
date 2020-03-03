<h1>Referências</h1>

* Sharma, S., & Coyne, B. (2013). DevOps for dummies. Limited IBM Edition’book.

* Kim, G., Behr, K., & Spafford, K. (2014). The phoenix project: A novel about IT, DevOps, and helping your business win. IT Revolution.

* Humble, J., & Farley, D. (2010). Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation (Adobe Reader). Pearson Education.

* Mendes, Marco - Blog sobre DevOps - https://marco-mendes.com/devops/

<h1>Pipelinas e Linhas de Montagem DevOps</h1>

* Pipelines DevOps
    * Tubulação - Tradução para Pipeline
    * Completar parte com fluidez
    * Mecanismos automatizados para reduzir o tempo de entrega de demandas, aumentar o feedback entre pessoas e também habilitar experimentos e inovações.

* Exemplo simples de pipeline
    * Build automatizado -> Tstes automatizados -> Entrega no ambiente de testes
    * Continous Integration

* Outro exemplo de pipeline
    * Provisiona ambiente com o Docker
    * Publica aplicação em conteiner Docker
    * Habilita contêiner em ambiente de produção

* Um terceiro exemplo de pipeline - SecOps
    * Identifica ambientes com vulnerabilidades -> Aplica patch de segurança de forma automatizada -> Gera dados analíticos para time de segurança.

* Linhas de montagem DevOps
    * As linhas de montagem DevOps estão focadas em automatizar e conectar atividades realizadas por várias equipes, como CI para desenvolvedores, provisionamento de infraestrutura e gerenciamento de configuração para operações, teste de automação para teste, patch de segurança para SecOps, portais de aprovação e versionamento semântica para gerentes de liberações e assim por diante.

* Benefícios de negócio de pipelines e linhas de montagem
    * Gatilhos automáticos ou aprovação manual entre pipelines ou centros de trabalho.
    * Métricas e análises em pipelines para ajudar a identificar gargalos.
    * Visibilidade em cada pipeline ou centros de trabalho.
    * Trilhas de auditoria.
    * Reduçao do tempo de execução para executar as tarefas nos centros de trabalho.
    * Capacidade de definir facilmente fluxos de trabalho em vários pipelines
    * Automação da infraestrutura de DevOps, incluindo VMs e containers.
    * Capacidade de transmitir estado e outras informações (feedback e feedfoward).

<h1>Automação de Builds e Integração Contínua (CI)</h1>

* Times tradicionais
    * Passam a maior parte do tempo de um projeto com o software sem funcionar.
    * Operam durante muito tempo com códigos isolados.
    * Adiam tarefas de integração e testes de aceite para o final do projeto.


* Ferramentas:
    * Jenkins, Gitlab

* A automação de builds é prática essencial para garantir que os executáveis dos seus produtos sejam gerados de forma consistente, em base diária. Esta prática busca evitar o problema comum do código funcionar apenas máquina do desenvolvedor.
* A automação de builds externaliza todas as dependências de bibliotecas e configurações feitas dentro de uma IDE para scripts e que possa ser consistentemente executado por robôs. Ela é pilar básico para avançarmos em direção a fluxos de CI.
* Embora a automação de builds, na sua definição inicial, lide apenas com a construção de um build, a prática comum de mercado é que builds devam executar um conjunto mínimo de testes de unidade automatizados (smoke tests) para estabelecerem confiabilidade mínima ao executável sendo produzido.
<img src="imgs/01.png"/>

* Você só terá integração contínua quando o número de builds for diários ou até menor.

* Requisitos para a Gestão de Builds
    * Acordos entre o time -> Gestão de configuração -> Compilação automatizada -> Checkins diários de código -> Testes de unidade automatizados -> Suíte abrangente de testes -> Processo leve de compilação e testes 

<h1>Exemplo Prático de Automação de Builds</h1>


* A automação de builds é prática essencial para garantir que os executáveis dos seus produtos sejam gerados de forma consistente, em base diária. Esta prática busca evitar o problema comum do código funcionar apenas máquina do desenvolvedor

* Azure Devops
* Exemplo de Automação de Builds
<img src="imgs/02.png"/>
<img src="imgs/03.png"/>
<img src="imgs/04.png"/>
<img src="imgs/05.png"/>


