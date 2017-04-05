# Caixa Branca

A técnica de **teste de caixa branca** (_white-box testing_) tem como objetivo avaliar a estrutura interna dos elementos de programação _(técnica estrutural)_ durante a etapa de [Codificação](/codigo/README.md) nas fases de **testes unitários** (_unit testing_) - responsáveis por auxiliar e avaliar no desenvolvimento dos cenários de uma unidade de código (estrutura interna do programa) e/ou **testes de integração ou componentes** (_integration testing or component testing_) - responsáveis por avaliar a comunicação entre unidades e recursos, principalmente a camada de infraestrutura e códigos de terceiros (**verificação**).

Durante o desenvolvimento de _software_, os testes auxiliam nas técnicas de:

* **Projeto de Programa Sistemático** - _Systematic Program Design_ (SPD);
* **Desenvolvimento Guiado por Testes** - _Test Driven Development_ (TDD);
* **Refatoração** - _Refactoring_;
* **Cobertura de Testes** - _Test Coverage_;
* **Integração Contínua** - _Continuous Integration_ (CI); e
* **Testes de Regressão** - _Regression Testing_.

Outras características apresentadas são:
* Implementação: das funcionalidade do cenário;
* _FeedBack_: notificação dos problemas no código;
* _Bugs_: previne e corrige os problemas; e
* _Debugging_: reduz a necessidade de uso.

## O Teste

O teste utiliza as tarefas do cenário para a composição de um conjunto de casos de teste durante a etapa de [Codificação](/codigo/README.md), assim descrevendo **o que** cada estrutura de programação deve fazer para garantir a **verificação** da [Arquitetura](/arquitetura/README.md).

Na elaboração dos casos de teste utiliza uma identificação e um nome descritivo para cada variação de uma específica funcionalidade do cenário - formando uma execução atômica, assim definindo seus dados de testes como entrada e sua saída esperada na execução, conforme o estado inicial.

`{ ID; Nome do Teste; Entrada; Saída Esperada; Estado Inicial }`

Os casos de teste são organizadas em quatro (4) fases/etapas, sendo:

* **setup** ou **arrange**: construção e configuração dos estados (entradas, condições e limites) requeridos pelo caso de teste;
* **exercise** ou **act**: execução das funcionalidades do código sobre teste;
* **verify** ou **assert**: avaliação dos estados e comportamentos do código, comparando os resultados obtidos com as saídas esperadas; e
* **teardown** ou **after**: liberação dos recursos utilizados pelo código.

**Importante o cuidado** para não violar o Princípio da Responsabilidade Única - _Single Responsibility Principle_ (SRP) durante a implementação do código sobre teste, pois deve-se testar apenas as funcionalidades expostas (_Tell, Don't Ask_) sem o encadeamento de mensagens (_Law of Demeter_), a proposta básica é que cada **Classe de Equivalência** deve possuir um caso de teste único e suficiente, ou seja, a inclusão de pequenos incrementos entre testes conforme suas condições limites.

### O Que Testar?

As tecnologias de desenvolvimento possuem elementos de programação mínimos legíveis aos testes, sendo:

* **Java**: Classes e Métodos;
* **Haskell**: Funções;
* **Lisp**: Funções, Comandos e Macros; e
* **C**: Funções.

### Documentação

Os testes formam a documentação viva do código, em que são de extrema importância seus identificadores (nomes dos testes) serem pensadas em nível sintático (relação entre os termos) e semântico (sentido de ideias) com o que será testado.

#### Convenções

As seguintes convenções para os identificadores são utilizados:

* Casos de Testes:

  * _NameTest_: testes unitários;
  * _NameIntegrationTest_: testes de integração; e
  * _NameSystemTest_: testes de sistema (ver [Caixa Preta](/testes/caixa-preta.md)).

* Testes:

  * _Action_: utiliza uma ação avaliável do teste, considerando o resultado e/ou condição da operação, exemplo: _adicionaUmUsuarioEmUmaListaVazia_;
  * _Given-When-Then_: relaciona o contexto, ação e resultado do teste, exemplo: _dadoXQuandoAcontecerYEntaoFacaZ_; e
  * _Helper Objects_: nomeia os comandos em modo imperativo e as avaliações em modo indicativo, exemplo: _dispareUmSinalDeFalha_ e _mostraAOcorrenciaDaFalha_.

#### Dicas

Os identificadores tendem a ficarem longo, assim dificultando em sua leitura - uma dica é utilizar _underscore_ sobre o _camel case_:

`requisitarUmaMensagemComRepositorioVazio` para `requisitar_uma_mensagem_com_repositorio_vazio`

### Feedbacks

Os excessos no código de teste (padrões de _feedback_) diz o quanto estável é a unidade de programação:

* exercícios das responsabilidades: baixa coesão;
* dublês das colaboradoras: alto acoplamento; e
* avaliação em colaboradoras: encapsulamento.

Complexidade ciclomática: métrica das ramificações existentes em uma unidade de programação, quanto maior o número, mais complexo e difícil de ser testado será o _software_ (mais informações em [Medindo a complexidade do seu código](http://blog.caelum.com.br/medindo-a-complexidade-do-seu-codigo/ "Medindo a complexidade do seu código")).

### Ferramentas

As [ferramentas](ferramentas.md) mais utilizadas são:

* assert
* JUnit
* Hamcrest
* Mockito

## A Prática

### Exceções

@Test:expected _em edição_

@Rules _em edição_

Try-Catch _em edição_

EAM _em edição_

## O que pensar?

* **AAA[A]** - organização e formatação dos casos de teste:

  **A**rrange: monta/organiza o código com todas as entradas e pré-condições necessárias ao teste;

  **A**ct: exercita/executa o código sobre teste;

  **A**ssert: avalia os resultados obtidos do código com os esperados pelo teste;

  **A**fter: finaliza os recursos utilizados no teste.

* **FIRST** - propriedades de bons testes:

  **F**ast: rápidos em sua execução, assim mais testes serão avaliados;

  **I**solated: isolados dos outros códigos, assim a verificação da falha será óbvia;

  **R**epeatable: possui repetibilidade em qualquer ordem e tempo;

  **S**elf-validating: testes autoavaliáveis, automação em sua execução e avaliação;

  **T**imely: em momento oportuno, escreva os testes antes do código.

* **R-&gt;BICEP** - questões sobre os testes:

  **R**ight: os resultados estão certos?;

  **B**oundary: as condições limites estão corretas? Essa é verificada através do **CORRECT**;

  **I**nverse: os relacionamentos inversos (operações inversas) estão sendo utilizadas?;

  **C**ross-Check: uso de checagem cruzada com outros métodos de mesmo significado estão sendo utilizadas?;

  **E**rror Conditions: as condições de erros estão sendo forçadas?;

  **P**erformance: o desempenho está dentro dos limites?.

* **CORRECT** - as condições limites estão:

  **C**onformance: com os valores conforme o formato especificado?

  **O**rdering: com o conjunto de valores em uma ordem determinada?

  **R**ange: com os valores dentro da faixa (mínimo e máximo) especificada?

  **R**eference: com alguma referência externa fora do controle do código?

  **E**xistence: com valor existente (nulo, zero, presente e etc...)?

  **C**ardinality: com a quantidade de números suficiente? Os casos interessantes são Zero, Um e Muitos através da regra **0-1-n**.

  **T**ime: com as temporizações corretas (sincronização, tempo, eventos, referência e etc...)?

## Boas Práticas

* **Identificação**: ver Documentação.
* **Refatoração**: importante até mesmo para o código de teste.
* **Baby Steps**: começando pelo cenário de teste mais simples em pequenos incrementos, assim ganhando confiança e conhecimento do sistema.
* **Test Data Builders**: utilização do padrão de projeto (GoF) _Builder_ para o processo de criação dos objetos para os cenários de testes - auxilia no problema de duplicação de código.
* **Adapters**: utilização para testes com métodos estáticos e códigos legados.
* **Test Double**: isolação de funcionalidades com dependência externa, assim avaliando as características de estado e comportamento do objeto:
  * _Dummy_: _em edição_.
  * _Fake_: _em edição_.
  * _Stubs_: _em edição_.
  * _Saboteurs_: _em edição_.
  * _Mocks_: _em edição_.
  * _Spy_: _em edição_.
* **Infraestrutura**: a camada de infraestrututra (_DAO_, _Messages_...) é testada com testes de integração.
* **Execute Around Method**: utilização para testes com avaliação de exceção.

### Test Smell

Código de teste também possui _bad smells_, tais como:

* **Unnecessary Test Code** (Código de Teste Desnecessário): o caso de teste é construído com código em excesso e/ou defensivo, sem significado e valor ao teste;
* **Missing Abstractions** (Falta de Abstração): exagero e/ou preciosismo nos detalhes sobre a organização e formatação do teste;
* **Irrelevant Information** (Informação Irrelevante): utilização de dados irrelevantes ao teste, tais como literais e sentinelas;
* **Bloated Construction** (Construção Inchada): complexidade na montagem dos elemento no teste;
* **Multiple Assertions** (Múltiplas Avaliações): excesso de responsabilidades no teste;
* **Irrelevant Details in Test** (Detalhes Irrelevante no Teste): uso de recursos desnecessários ao teste, tais como serviços transversais de segurança, _logging_ e etc...;
* **Misleading Organization** (Organização Enganosa): falta de organização no código de teste, por não responder a questão _AAA_;
* **Implicit Meaning** (Significado Implícito): excesso de dados e informações aos elementos (constantes, variáveis, dados e etc...) do teste;

