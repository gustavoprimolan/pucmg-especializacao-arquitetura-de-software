<h1>Unidade 04 - Estilos e Padrões Arquiteturais</h1>

<h2>Estilos Arquiteturais</h2>

<h3>Estilos Arquiteturais</h3>

* Estilos e padrões arquiteturais são estilos de padrões de projetos que podem ser reutilizaveis.
* São resolvidos dentro de um contexto especifico.
* Nesse cenário é importante lembrar que muitas vezes os problemas se repetem.
* Suas características se encontram em contextos de sistemas diferentes.
* Diante de problemas semelhantes, podemos usar padrões arquiteturais ja validados e conhecidos como solução para esses problemas.
* Forma um conhecimento comum e compartilhado.
* Existem diferentes estilos arquiteturas e incluse o nome entre autores diferentes.
* Alguns autores vão citar mais ou menos estilos de padrões arquiteturais.
* Muitos autores podem agrupar estilos e padrões.
* O importânte é entender e saber entender qual padrão utilizar ao problema que temos em questão.

<img src="imgs/01.png"/>

* Elementos que caracterizem a arquitetura.
* Não são uma arquitetura de software completa, mas sim o primeiro passo para desenho ou definir qual vai ser a arquitetura do sistema. Solução inicial, preconcebida.
* Normalmente utilizada em algumas situações.

* Classificação de Padrões Arquiteturais
    * Vários parâmetros podem ser usados:
        * Forma de passagem de controle entre componentes: Sistemas de fluxo de dados ou Padrões de comunicação (síncrono x assíncrono).
        * Ênfase em atributos de qualidade (manutenibilidade ou desempenho).
    * Sistema deve:
        * Atender requisitos funcionais.
        * Atender requisitos não funcionais: Portabilidade, Manutenabilidade, Estabilidade, Confiabilidade, Desempenho.

<h3>Arquitetura em Camadas</h3>

* Maneira comum de documentar arquitetura de software
* Ajudam a decompor as aplicações que podem ser subdividas em subgrupos por tarefa.
* Exemplo classico seris os protocolos de rede.
* Na divisão desses protocolos ocorrem a descrição de como a comunicação se da entre as diversas camadas.
* Importante definir contato, conteudo e significado das mensagens que são trocadas entre as camadas, cenarios precisam ser descritos em detalhe
* Cada camada terá um responsabilidade.
* Cada camada realizará um trabalho que será aproveitado na camada seguinte.
* Um contexto de uso seria um sistema grande e complexo que vai demandar algum tipo de decomposição, algum tipo de quebra que vai demandar responsabilidades diferentes.
* Como seria um implementação em arquitetura em camadas?

* Implementação
    * 1 - Defina o critério de abstração para agrupar tarefas em subcamadas
    * 2 - Determine o número de níveis de abstração.
    * 3 - Nomeie as camadas e assinale tarefas a cada uma.
    * 4 - Especifique os serviços. Camadas devem ser totalmente separadas uma da outra.
    * 5 - Refine as camadas.
    * 6 - Especifique uma interface para cada camada.
    * 7 - Estruture camadas individuais.
    * 8 - Especifique os mecanismos de comunicação entre elas.
    * 9 - Projete uma estratégia de gerência de erros.

* Benefícios
    * Reuso de camadas.
    * Suporte para padronização.
    * Dependências são mantidas localmentes dentro da propria camada
    * Manutenibilidade
        * Camada pode ser trocada facilmente
        * Exemplo: hardware

* Desvantagem
    * Desempenho

<h3>Sistemas Interativos</h3>

* São baseados em um conjunto de requisitos funcionais
* Uso mais intencivo das interfaces de usuário
* Necessidade de alteração com certa frequencia
* Possibilidade que alterações da interface sejam executadas sem impactar o cumprimento e atendimento dos requisitos funcionais.
* Modelos comuns: Modelo MVC

* Modelo MVC
    * Divide aplicação em 3 componentes:
        * Modelo: Funcionalidade básicas e dados.
        * Visão: Exibe informação ao usuário.
        * Controle: Gerenciam entrada e dados.
    * Usado em aplicações interativas que tem uma interface gráfica com o ator humano mais flexivel.
    * Podendo mexer a mesma informação de diversas formas, sem impactar na informaação que esta por trás.
    * Sistemas interativos como o modelo MVC precisam suportar o Look-and-feel diferentes.
    * Look-and-feel trata da aparencia das aplicações. A interface precisa refletir mudanças nos dados imediatamente.
    * Trata-se de um conceito chamado de Separation of concerns.
    * Cada uma dessas estruturas do MVC vai ter uma responsabilidade diferente e separada.
    <img src="imgs/02.png"/>

    * Visão:
        * Componentes são responsáveis por exibir a informação ao usuário
        * Cada visão vai ter associada a ela um componente de controler para ela realizar essa visão.
        * Responsabilidade da visão capturar movimentos do mouse e cliques, etc.
    * Controllers
        * Recebem entradas que forem executadas pela visão
        * Determina com base na entrada o que o usuário deseja fazer.
        * Faz a comunicação de volta com a visão para o que o cliente deseja ver
    * Model
        * Modelo contem ou representa o núcleo dessa aplicação
        * Propagação de mudanças
        * Definir de como os dados serão tratados.
        * Objetos da aplicação
        * Instancias mostram os estados da aplicação

* Modelo MVC - Controle
    * Frameworks de aplicação que podem ser usados na camada de controle:
        * Struts.
        * Java Server Faces.
        * Spring.
        * WebWork

* Benefícios
    * Múltiplas visões do mesmo controle.
    * Visões sincronizadas (mecanismo de propagação).
    * Controles e visões são "plugáveis".
    * Substituição fácil  de "look and feel".
    * Desenvolvedores da interface gráfica poderem focar exclusivamente no seu trabalho, sem se preocupar com lógica do negócio.
    * Desenvolvedores vão focar na implementação da lógica dos negócio sem se preocupar com recursos de interface gráfica.


<h3>Sistemas Distribuídos</h3>

* Cenário comum para sistemas distribuidos seria um sistema rodando em várias CPU's
* Redes conectando vários computadores.

* Vantagens
    * Economia, Desempenho e Escalabilidade (usam recursos distribuídos na rede).
    * Confiabilidade (uma máquina pode falhar sem afetar o restante do sistema).

* Desvantagens
    * Precisam de software específico.

* Um dos padrões para se trabalhar com sistemas distribuidos é o padrão Broker.
    * Pode ser utilizado para estruturas sistemas de software que possuem chamadas remotas.
    * Existe um componente chamado Broker que é responsável por coordenar a comunicação, assim como enviar a solicitações e transmitir resultados e exceçõs tratadas entre os componentes.

<img src="imgs/03.png"/>

* Padrão Broker
    * Componente Broker atua para separar melhor clientes de servidores.
    * Servidores:
        * Se registram no broker.
        * Tornam seus serviços disponíveis a clientes através de interfaces definidas.
    * Clientes:
        * Acessam funcionalidades dos servidores através de requisições ao broker.
    * Arquitetura broker precisa ser flexível
        * Objetos podem ser alterados facilmente
    * Precisa fornecer apis de comunicação aos seus clientes.
    * Responsabilidades do componente broker:
        * Localizar o servidor apropriado.
        * Reenviar solicitações aos servidores.
        * Transmitir resultados e exceções aos clientes.

* Conhecidos do padrão broker podem ser vistos como CORBA
* CORBA - Common Object Request Broker Architecture
    * Tecnologia orientada a objetos para distribuir objetos heretogeneos.

* WWW
    * Navegadores atuam de certa forma como brokers
    * Servidores WEB atuam como provedores de serviço.

<h3>Outros padrões arquiteturais</h3>

* Nomenclatura aos estilos arquiteturais é um pouco adversa.
* Primeiro estilo:
* Sistemas de fluxos de dados:
    * Possuem dois ou mais componentes de processamento;
    * Transformam dados de uma entrada em dados de uma saída.
    * Transformação de maneira sequencial.

    * Pipes and filters
        * Uma componente de processamento tem duas saídas.
            * Saída padrão
            * Saída de erro.
        * Mecanismos de entradas e saída são chamados portas.
        * Um filtro típico possui três portas.
    <img src="imgs/04.png"/>
    <img src="imgs/05.png"/>

    
* Sistemas de chamada e retorno
    * Caracterizados por um processo inicial de controle que invoca operações.
    * Utilizado em sistemas orientados a objetos.
    <img src="imgs/06.png"/>

* Componentes independentes
    * Componentes independentes dependem de chamada implícita de operações.
    * Chamada da operação está desconectada da execução.
    * Componente "chamador" e "chamado" podem existir em processos separados e até mesmo em processadores distribuídos.
    * Tendem a ser mais modulares.
    * Mais possibilidade de reuso.
    * Sistema em si é mais complexo normalmente.
    * São uma forma de sistema distribuído.
    * Sujeitos a restrições de desempenho.
    
    <img src="imgs/07.png"/>

* Repositórios
    * Envolvem fonte de dados compartilhada.
    * Motivação: Guardar dados persistentes.
    * Dois elementos principais:
        * Elemento de dados central;
        * Múltiplos elementos processadores independentes.

    * Quadro Negro (Blackboard)
        * Do tipo repositório.
        * Fonte de conhecimento: elementos processadores.
        * Quadro negro: elemento central compartilhado.
            * Exemplo: Sistema de banco de dados.
        <img src="imgs/08.png"/>

* Peer-to-Peer
    * Cada um dos membros funcionam como um par um do outro.
    * Todos eles atuam tanto como clientes como servidores
    <img src="imgs/09.png"/>
    * Aplicação:
        * Distribuição de arquivos
        * Processamento - Compartilhar processadores.

* Taxonomias
    * A classificação dos estilos arquiteturais pode variar de acordo com a referência bibliográfica.
    * São apresentados a seguir alguns resumos de tais classificaçoes.
    <img src="imgs/10.png"/>
    <img src="imgs/11.png"/>
    <img src="imgs/12.png"/>

<h2>Serviços</h2>

<h3>Introdução a Serviços</h3>

* Conceito não é novo.


<h2>Tópicos em estilos arquiteturais</h2>