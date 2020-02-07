<h1>Introdução</h1>

- Qual o papel das visoes e estilos arquiteturais?

  - Impossível representar todas característicos em um único estilo arquitetural.
  - As visoes e os estilos arquiteturais devem ser utilizados de forma a documentar partes específicas da arquitetura.
  - Visao de Modulos

    - Decomposicao
    - Usa
    - Generalizacao
    - Camadas
    - Aspectos
    - Repositórios de dados compartilhados.

  - Visao de Componentes e Conectores

    - Pipe e filtro
    - Cliente-servidor
    - Ponto a ponto
    - Arquitetura Orientadas a Serviços
    - Publicador-assinante

  - Visao de Alocação

    - Implantação
    - Instalação

  - Documentacao de Interfaces
  - Como documentar arquitetura usando a UML

<h1>Visão de Módulos</h1>

<h1>Práticas de documentação de arquitetura de software</h1>

- Regras de uma boa documentação

  - Use o ponto de vista do leitor.
  - Evite repetições
  - Evite ambiguidade.
  - Siga um template padrao.
  - Registre as motivacoes
  - Mantenha a documentacao atualizada.
  - Revise a documentacao.

- Notações

  - Informais

    - Caixas e setas;
    - Descricoes em linguagem natural.

  - Semiformais

    - UML

  - Formais
    - ADLs (Architecure Description Languages).

- Notações Informais

  - C1 -> C2
  - O que significa a seta?
    - C1 chama C2
    - Existe fluxo de dados em C1 para C2
    - C1 envia mensagem para C2
    - C1 instnacia C2
    - C1 É SUBTIPO DE c2
    - C2 é um repositório de dados e C1 escreve em C2.
    - C1 é um repositório de dados e C2 le de C1.

- Estilos x Padrões

  - Padrão Arquitetural = {problema, contexto}
    - Abordagem Arquitetural.
  - Estilo Arquitetural = Abordagem Arquitetural.

- Tipos de visões

  - Visão de módulos

    - Estrutura.

  - Visao de componentes e conectores

    - Comportamento em tempo de execução.

  - Visão de alocação
    - Distribuiçao dos elementos de software.

<h1>Visao de Módulos I</h1>

- Módulo

  - Unidade de implementação de software que prove um conjunto coerente de responsabilidades.

- Responsabilidade

  - Papel que o módulo assume para atender os atributos de qualidade ou a funcionalidade de um sistema.

- Relações

  - É-parte-de (agregações);
  - Depende-de (usa, permitido-usar, crosscuts);
  - É-um (especialização/generalização).

- Propriedades

  - Regras para:
    - Guiar a implementação do módulo;
    - Analisar os módulos e suas relações.

- Estilos associados a visao de módulos
  - Decomposicao
  - Usa
  - Generalizacao
  - Camadas
  - Aspectos
  - Modelo de Dados

<img src="imgs/01.png"/>

- Decomposição
  - Usado para decompor um sistema em módulos.
  - Mostra
    - Agregações entre módulos;
    - Hierarquia de decomposições de módulos.
  - Relação: é-parte-de.
  - Propriedades/Restrições:
    - Nao podem existir ciclos
    - Cada módulo só pode ter um pai

<img src="imgs/02.png"/>

<img src="imgs/03.png"/>

- Usa
  - Mostra dependencias entre módulos.
  - Relação: depende-de.
  - Usado para planejar incrementos/subconjuntos de desenvolvimento.
  - Propriedades:
    - Evitar uso de ciclos.
      <img src="imgs/04.png"/>
    - Evitar uso de fan-out largos.
      <img src="imgs/05.png"/>
    - Evitar longas cadeias de dependencias.
      <img src="imgs/06.png"/>
  - Nao esperessam necessariamente o estilo:
    - Chamadas entre módulos;
    - Inclusao de módulos.
      <img src="imgs/07.png"/>
      <img src="imgs/08.png"/>
      <img src="imgs/09.png"/>

<h1>Visão de Módulos II</h1>

- Generalização

  - Utiliza a relação é-um.
    - Permite extensão e evolução da arquitetura do software.
  - Módulos organizados para expressarem parte comuns e variações.
  - Módulos podem ser abstratos.
  - Propriedades / Restrições:
    - Módulos podem possuir mais de um pai (design perigoso).
    - Não se permite ciclos nas relações de generalização.
  - Deve ser usado para:
    - Permitir extensão e evolucao da arquitetura de forma incremental.
    - Capturar características comuns e representar as variações nos módulos filhos.
    - Dar suporte ao reuso.
      <img src="imgs/10.png"/>

- Camadas
  - Divisão em unidades de chamadas camadas
    - Conjunto de módulos;
    - Interface bem definida.
  - Relação: permitido-usar
    - Especialização da relação depende-de.
  - Propriedades / Restrições:
    - Relação unidirecional.
    - Acíclica.
    - Cada módulo pertence a uma única camada.
  - Relação de ordem:
    - Camadas Superiores podem usar camadas inferiores;
  - Se (A,B) são camadas.
    - A é permitida-usar os serviços de B através de sua interface.
  - Usado para promover:
    - Modificabilidade e portabilidade;
    - Reuso;
    - Speração de interesses ou preocupações;
    - Testabilidade.
  - Camadas nao existem em tempo de execução.
    - Mecanismos de organização e abstração do projeto.
      <img src="imgs/11.png"/>
      <img src="imgs/12.png"/>

* Aspectos
  - Módulos são aspectos que representam interesses cruzados.
  - Relação: Crosscuting concerns.
  - Restrições / Propriedades:
    - Um aspecto pode ter relação de crosscuting concern com outros aspectos ou com módulos regulares.
  - Um aspecto não deve ter relação de crosscuting concern com ele mesmo.
  - Usado para melhorar a modificabilidade da arquitetura.
    - Evita que a funcionalidade do domínio e a dos crosscuting concerns seja distribuída entre diversos objetos.
      <img src="imgs/13.png"/>
      <img src="imgs/14.png"/>
      <img src="imgs/15.png"/>

<h1>Visão de Componentes e Conectores</h1>
