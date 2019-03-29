<h1>Unidade 02 - Práticas de arquitetura de software</h1>
<h2>Documento de Arquitetura</h2>

<h3>Arquitetura no RUP</h3>

* RUP é o processo unificado da racional, é um processo tradicional, prescritivo, que indica ao desenvolvedor, a equipe quais atividades devem ser feitas e prove também templates para essas atividades.
* RUP é um exemplo de processo tradicional.
* No RUP, a arquitetura de software (em um determinado ponto) é a organizacao ou a estrutura dos componentes significativos do sistema que interagem por meio de interfaces, com elementos constituídos de componentes e interfaces sucessivamente menores.
* A Arquitetura é formada por um conjunto de componentes, precisamos entender quais são esses componentes menores que compõem o sistema.
* Esse componentes se comunicam por meio de interfaces.
* Teremos sempre componentes e interfaces sucessivamente menores o que nos da uma ideia de refinamento, a arquitetura é definida a principio de uma maneira mais macro, pensando em todos os componentes. Com o passar do tempo a medida que vamos entendendo e definindo os componentes maiores, vamos pensando então nos elementos maiores. A arquitetura é refinada.
* Como o projeto restabelece o fluxo de trabalho a cada iteração a arquitetura é desenvolvida, refinada e aprimorada. O RUP parte da ideia que os processos podem ser iterativos, vamos lembrar do gráfico das baleias que mostra como é concentrado em cada uma das etapas do RUP. Em cada uma das suas disciplinas, como o esforço se divide ao longo das fases. Nesse sentido a arquitetura dentro do RUP, esta dentro do fluxo de analise de desenho pode ser executada a qualquer momento do projeto.
* Os esforços de arquitetura tendem a se concentrar no inicio do projeto, na iniciação e na elaboração principalmente, não querendo dizer que pode iniciar em outra fase.
* Com cada interação inclui a integração e o teste, sendo uma arquitetura bastante sofisticada.
* Esta arquitetura é o enfoque principal das iterações da fase de elaboração.
* O principal objeto da fase de elaboração muitos pensam que é chegar uma especificação de requisitos pronta, definida ou detalhada. Isso acontece em boa parte, mas o principal objetivo da fase de elaboração do RUP é terminar a arquitetura.
* É chegar com a arquitetura ja pronta, validada. Ao final dessa fase a arquitetura vai estar analisada.
* No RUP esta previsto tbm um artefato chamado de estilo de arquitetura. Vimos que algumas empresas termos arquiteturas padrão ou arquiteturas de referencia, nesse caso então o estilo de arquitetura vai ajudar a reduzir o conjunto de formulários ou artefatos e vai impor um certo grau de uniformidade a arquitetura, um grau de padronização.
* Estilo de Arquitetura no RUP
    * Pode ser definido por um conjunto de padroes, ou pela escolha de componentes ou conectores específicos que vai funcionar com esses elementos básico para a construção da arquitetura.
	Esse estilo vai nos ajudar a padronizar e formalizar a arquitetura.
    * Um determinado sistema, podemos utilizar alguns estilos como parte da descrição da arquitetura.
    * No RUP vai prever um documento chamado guia de design ou guia de desenho ou guia de projeto. Esse guia vai mostrar e definir um estilo e esse estilo vai ter um papel vital na compreensão e na integridade da arquitetura desse sistema.
	* Fluxo de Analise de desenho.
	* Quando o fluxo se inicia, pode haver iteração na fase de iniciação. Uma iteração opcional, nesse sentido pode ser executado uma atividade chamada Realizar síntese arquitetural. Isso acontece por conta de que na iniciação pode haver informações que podem ser utilizadas em uma primeira documentação, ou para uma primeira analise ou primeiro entendimento da arquitetura no sistema. Caso isso seja possível na iniciação, essa etapa/atividade vai ser executada.
	* Se não, na fase de elaboração nos temos uma atividade chamada definir uma sugestão de arquitetura. Arquitetura deve ser selecionada. Precisamos pensar em um conjunto de opções e selecionar e identificar uma melhor composição de arquitetura dentro dessas sugestões.
	* Existe também uma atividade de refinamento da arquitetura, a arquitetura é pensada em um nível mais macro e depois pensada em um nível mais micro, para refinamento.
	* Existem outras atividades que talvez reflitam mais atividades relacionadas a tesenho e ate mesmo a banco de dados. Como analisar comportamento, projetar componentes e projetar o banco de dados.
	* Nas organizações os nomes dos papeis que executam essas atividades variam. É comum ter nas organizações que chamam esse papel de projetista, outras podem chamar de arquiteto, líder técnico.
	* Essas atividades quando trazidas no contexto de uma organizacao, podem ser atribuídas a papeis diferentes. Esse fluxo de analise e desenho abrigam essas atividades que Possivelemnte vai ser executadas por arquitetos, por lideres técnicos, por projetistas, analistas de sistemas ou analistas de bancos de dados.
	* Existe uma outra figura em quais atividades o arquiteto de software participa no RUP.
	* Na parte central da figura, mostra as atividades que o arquiteto podem executar.
	* Na parte de cima e superior e inferior o arquiteto ajuda a produzir ou produz diretamente.
	* A principal saida da arquitetura seria o documento de arquitetura de software.
    * Podemos ver na parte superior no centro da figura. Vamos falar mais desse documento adiante. Temos também outro artefato importante, como arquitetura de referencia.
	* Arquitetura de referencia deve ser documentada e bem detalhada para que ela possa ser reutilizada e bem compreendida nos próximos projetos.

<h3>Documento de Arquitetura</h3>

* Um Documento de Arquitetura pode ser elaborado de diferentes formas e pode conter informações diferentes. Cada organização se preocupa ou precisa documentar diferentes tipos de informação. Entretanto, algumas informações são típicas em boa parte dos documentos que vemos no mercado.
* Documento importante, elaborado pelo arquiteto de software para comunicar e detalhar a arquitetura do sistema.
* O documento de arquitetura registra as principais decisões relacionadas a arquitetura de um software.
* Estabelece como esse sistema esta organizado. Quais são seus componentes internos e como esses componentes se comunicam e interagem entre si.
* Serve como mecanismo de comunicação entre a equipe.
* Os desenvolvedores vao consultar esse documento para conhecer melhor a arquitetura do sistema e em suas implementações estarem aderentes ou conforme essa arquitetura utilizada.
* Os analistas podem utilizar essa arquitetura também para verificar ou validar as informações que foram colocadas em suas especificações e outros papeis podem utilizar esse documento sempre que necessário.
* O documento de arquitetura vai ser definido por cada organizacao ou por cada projeto, claro que em organizações que possuem  uma metodologia de desenvolvimento de software ja estabelecida padronizada. Esse documento de arquitetura ja vai possuir um padrão. Esse processo, a metodologia da organizacao, vai dizer quando esse documento de arquitetura precisa ser produzido dependendo das características do projeto e quais as informações que são obrigatórias para esse documento.
* Vai também assinalar o momento, uma atividade em que esse documento vai ser realizado e também um papel responsável pela realização desse documento.
* Mesmo existindo a possibilidade de variações entre as organizações, mesmo a gente tendo o processo rup, o processo unificado que nos tras um padrão para trabalharmos arquitetura em projetos tradicionais, podemos destacar algumas sessões típicas em documentos de arquitetura.
* Normalmente um documento de arquitetura vai começar com uma sessão introdutória. Nessa sessão podem ser apresentadas informações relacionadas ao escopo do sistema
* Escopo - Claro que esse documento pode referenciar um documento de requisitos de especificação que ja tenha sido produzido, ou qualquer outro documento que contem informações de escopo.
* Definicoes e siglas dos termos utilizados.
* Referencias - Por ser um documento tecnico, na sua construção podem ser usados outros documentos mais técnicos, ate mesmo livros na literatura em geral. Posso fazer referencias a documentos entregues pelo cliente.
* Contexto do sistema - Contexto que o sistema esta sendo desenvolvido.
* Muitos acham que o documento de arquitetura é basicamente um conjunto de diagramas. Nao há necessidade de pensar dessa forma.
* O documento de arquitetura tem sim seus diagramas, mas ele deve ter também um bom texto de apoio, explicando qual é o contexto, explicando qual é o cenário de desenvolvimento desse projeto, desse software.
* Pode ter ainda tbm uma explicação sobre a estrutura do documento, como um sumario.
* Estrutura do Documento - O que é tratado em cada uma das sessões desse documento.
    * Esse documento vai ter ainda uma lista para apresentar os requisitos que são arquiteturalmente relevantes para o sistema. Provavelmente vamos encontrar os requisitos não funcionais que tem um impacto na arquitetura. Que ira nos auxiliar a definir a arquitetura.
	Os requisitos podem ser trazidos para ca, podem ser explicados aqui ou podemos referenciados um outro documento onde os requisitos estão escritos.
* É uma boa prática registro de requisitos e cada requisito tem um código único, justamente que possamos rastrear e identificar melhor esses requisitos. Claramente vai ser tratados aqui questões relacionadas a tamanho do software e a desempenho. Tamanho em sentido a quantidade de usuários, volume de dados que o software deve tratar e com qual desempenho, alem dos outros  tipos de requisitos nao funcionais que por ventura existirem nesse sistema.
* O documento de arquitetura vai trazer então as visões de arquitetura. Lembre-se que utilizamos o modelo 4 + 1 das visões arquiteturais.
* Sera mostrado as visões logica, visão de implantacao, visão de processos, visão de implementação e a de casos de uso.
* Essas visões são explicadas e detalhadas e serão tbm ilustradas com diagramas, provavelmente os diagramas da uml em sessões especificas desse documento.
* Diagrama de implantação vai ser usada na visão de implantação, diagrama de pacotes e componentes, provavelmente vai aparecer na visão logica ou na visão de implementação. Os diagramas de uml vistos, eles encaixam muito bem, são usados nesses contextos das visões.
* Algumas empresas também documentam essas visões sem o uso de diagramas uml. É comum vermos outros diagramas. Nao usam uma anotação padronizadas, mas que tbm são fáceis de entender, que podem ser usadas para documentar essas sessões e mostrar a arquitetura internamente.
* Um documento de arquitetura pode trazer alguma informação relacionada a persistência dos dados.
* Existem modelos para tratar essa persistência, como os dados serão registrados no sistema, na base de dados.
* Temos uma visão de dados do sistema. Nessa visão a preocupacao do arquitetura é documentar como esse mecanismo de persistência é utilizado, do ponto de vista para facilitar a vida do desenvolvedor. Podem ser mostrados inclusive exemplos de usos desses mecanismos para que os desenvolvedores tenham o seu trabalho facilidade ao implementar um código especifico de um caso de uso, por exemplo.
* E ainda, em um documento de arquitetura, pode haver uma explicação sobre algum framework utilizado. Bastante comum herdarmos algo ja reuzado, ja utilizado na empresa.
* Uma coisa importante é nao faltar detalhes da arquitetura, que é importante, tanto em quesito a diagramas e informações textuais.

<h3>Visoes Arquiteturais</h3>

* Sao importantes para a documentação de uma arquitetura de um sistema. A representação da arquitetura de um sistema vai ocorrer em varias visões, em varias representacoes.
* Cada uma dessas visões vai abordar um conjunto de questões especificas, para os envolvidos nos processos de desenvolvimento de software. Assim, algumas visões vao ser mais de interesse dos usuários finais, outras dos projetistas ou dos analistas, outras dos gerentes e outras dos desenvolvedores.
* Modelo de visão de arquitetura comentada é o modelo chamado quatro mais 1 (4+1), ele trás quatro visões, mais uma visão que seria a visão de caso de uso.
    * Visão Logica -> Usuario Final
    * Visto de Implementação -> Programadores
    * Visão de Processo -> Integradores de Sistemas
    * Visão de Implantação -> Engenharia de Sistemas	
    * Visão de Caso de Uso. -> Analistas

<img src="imgs/01.png"/> 

* Cada uma dessas visões mostra um componente, um detalhamento do sistema sobre um ponto de vista.
* A primeira visão é a Visão de Casos de Uso -> A Visão de casos de uso contem casos de uso e cenários que abrangem comportamentos significativos em termos de arquitetura, classes ou riscos técnicos.
* Nesse cenário não é necessário mostrarmos talvez todos os casos de uso do sistema. O Arquiteto vai ter a preocupação de mostrar os principais ou aqueles mais críticos que exigem uma integração. 
* Alguns requisitos são chamados de requisitos arquiteturalmente relevantes. Esses requisitos apresentam um desafio para a arquitetura ou eles determinam a arquitetura do sistema.
* Alguns desses casos de uso que contem ou implementam esses requisitos mais relevantes do ponto de vista da arquitetura serão mostrados aqui na visão de casos de uso. Se quisermos uma visão completa de todos os casos de uso, isso vai estar em um documento datalhado de casos de uso ou uma especificacao de requisitos de software.
* Aqui os casos de uso vai ser aqueles que afetam a arquitetura ou que trazem riscos técnicos. Riscos de integração, de comunicação, riscos relacionados a alguma requisito não funcional como tratar ou alcançar algum desempenho determinado.
* Casos de Uso ->
    * A visao de casos de uso contem casos de uso e cenários que abrangem comportamentos significativos em termos de arquitetura, classes ou riscos tecnicos.
    * Afetam a arquitetura em relacao a riscos.

* Elementos da visão de casos de Uso ->
	* Modelo de Casos de Uso
	* Pacote de nivels superior -> Agrupar pacotes de casos de uso relacionados. Casos de usos acionados pelos mesmos atores ou casos de uso no mesmo nível de complexidade, ou de um modulo do sistema.
	* Representação de atores e casos de uso mostrando quais atores acionam ou interagem com casos de uso.
    * Casos principais do ponto de vista da arquitetura.

<img src="02.png"/>
<img src="03.png"/>


* Visão Logica - A visao logica contem classes de design mais importantes e sua organizacao em pacotes e subsistemas. Contem algumas realizadoes de casos de uso. É um subconjunto do modelo de design.
    * Algumas empresas tratam algumas informações dentro de um documento de arquitetura, as vezes outras empresas tem tbm esse documento, como documento de desenho que traria tbm algumas dessas informações ate mesmo essas realizações desses casos de uso.
    * A realização do caso de uso poderia ser feita talvez mostrando um diagrama de sequencia da UML, ela mostra como que o fluxo como as informações correm dentro do sistema. Passando por diversas camadas ou atores ou classes diferentes.
    * Os casos de uso mostrariam a execução de um cenário de um caso de uso de um ponto de vista mais interno, não daquele ponto de vista mais externo, pensando no foco no usuário.
    * Alguns elementos que podem ser visto na visão logica:
	    * A visão logica pode ter pacotes, também de níveis superior
	    * Subsistemas de Design.
	    * Pacotes podem se quebrar ou agrupar classes ou relizacoes de casos de uso.

<img src="04.png"/>

* Visão de Implementação - A Visão de Implementação contem uma visão geral do modelo de implementação e sua organizacao em termos de modelos em pacotes e camadas.
	* Comum termos diversos frameworks que trabalham com estruturas de camadas especificas. Essa visão de arquitetura documentaria como é essa estrutura em camadas.
	* O diagrama mostra como a integração entre os componentes ocorrem.

<img src="05.png"/>

* Visão de Processos - A visão de processos contem a descrição das tarefas (processo e threads) envolvidas, suas interações e configurações, e a alocação dos objetos e classes de design em tarefas. Essa visão só precisará ser usada se o sistema tiver um grau significativo	de simultaneidade.
	* Nao é uma visão comum nos sistemas comerciais.
	* Muitas vezes essas empresas tratam como algo opcional que vai ser feitos normalmente quando o sistema apresentar essas características.
    * As threads tem maior maior, menor menor.
<img src="06.png"/>

* Visão de Implantação - A visão de implantação contem a descrição dos varios nos fisico da maior parte das configurações comum da plataforma e como as tarefas são alocadas na visão de processos nos nós fisico. Essa visão só precisara ser usada se o sistema estiver distribuído.
    * Na visão de implatacao é usado o diagrama de implatacao ou de distribuição da Url
	* Documento de arquitetura.
<img src="07.png"/>
	
* Se existe um documento de arquitetura, a empresa ira documentar essas visoes, sendo uma parte substancial de um documento de arquitetura das organizacoes.

<h3>Documento de Arquitetura</h3>

* Um Documento de Arquitetura pode ser elaborado de diferentes formas e pode conter informações diferentes. Cada organização se preocupa ou precisa documentar diferentes tipos de informação. Entretanto, algumas informações são típicas em boa parte dos documentos que vemos no mercado. Nesta vídeoaula, apresentamos um pouco do que pode ser considerado uma estrutura típica de documentação de arquitetura.

