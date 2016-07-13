# Caixa Branca

A técnica de **teste de caixa branca** \(_white-box testing_\) tem como objetivo avaliar a estrutura interna dos elementos de programação _\(técnica estrutural\)_ durante a etapa de Codificação nas fases de **testes unitários** \(_unit testing_\) - responsáveis por auxiliar e avaliar no desenvolvimento dos cenários de uma unidade de código \(estrutura interna do programa\) e\/ou **testes de integração ou componentes** \(_integration testing or component testing_\) - responsáveis por avaliar a comunicação entre objetos e recursos, principalmente a camada de infraestrutura e código de terceiros.

Na etapa de Codificação, os testes de caixa branca auxília nas práticas do _Extrema Programming_ \(XP\):

* **Desenvolvimento Guiado por Testes** - _Test Driven Development_ \(TDD\): empregra os testes como a _principal ferramenta de codificação_, antes mesmo do código de produção, através do seu ciclo:

  * _Red_: o teste representa cada incremento do requisito;
  * _Green_: o teste guia a implementação do código; e
  * _Refactor_: os testes mantém a integridade do código.

* **Integração Contínua** - _Continuous Integration_ \(CI\): auxilia na execução automática e avaliativa dos testes;

* **Testes de Regressão**: auxilia na validação do código novo e\/ou alterado;

* **Cobertura de Testes**: auxilia na métrica dos testes; e

* **Refatoração**: auxilia na verificação da funcionalidade do código, antes e depois da modificação.


**Importante o cuidado** para não violar o Princípio da Responsabilidade Única - _Single Responsibility Principle_ \(SRP\) durante a implementação do código sobre teste, pois deve-se testar apenas as funcionalidades expostas \(_Tell, Don't Ask_\) sem o encadeamento de mensagens \(_Law of Demeter_\), a proposta básica é que cada **Classe de Equivalência** deve possuir um caso de teste único e suficiente, ou seja, a inclusão de pequenos incrementos entre testes conforme suas condições limites.

## O Teste

O teste utiliza um cenário \(requisito\) para composição de um conjunto de casos de teste durante a etapa de Codificação, assim garantindo a estrutura dos elementos de programação.

Os casos de teste são organizadas em quatro \(4\) fases\/etapas - pensando na sigla **AAA\(A\)**, sendo:

* **setup**: construção e configuração dos estados \(entradas, condições e limites\) requeridos pelo caso de teste;
* **exercise**: execução das funcionalidades do código sobre teste;
* **verify**: avaliação dos estados e comportamentos do código, comparando os resultados obtidos com os esperados; e
* **teardown**: liberação dos recursos utilizados pelo código.

### O Que Testar?

As tecnologias de desenvolvimento possuem elementos mínimos para testes, sendo:

* **Java**: Classes;
* **Lisp**: Funções, Comandos e Macros; e
* **C**: Funções.

### Documentando

Os testes formam a documentação viva do código, em que são de extrema importância seus identificadores \(nomes dos testes\) serem pensadas em nível sintático \(relação entre os termos\) e semântico \(sentido de ideias\) com o que será testado.

#### Convenções

Os seguintes identificadores são utilizados para os:

* Casos de Testes:

  * **NameTest**: testes unitário;
  * **NameIntegrationTest**: testes de integração; e
  * **NameSystemTest**: testes de sistema \(ver [Caixa Preta](caixa_preta.md)\).

* Testes:

  * **Action**: utiliza uma ação avaliável do teste, considerando o resultado e\/ou condição da operação, ex: _adicionaUmUsuarioEmUmaListaVazia_; e
  * **Given-When-Then**: relaciona o contexto, ação e resultado do teste, ex: _dadoXQuandoAcontecerYEntaoFacaZ_.


#### Dicas

Os identificadores tendem a ficarem longo, assim dificultando em sua leitura - uma dica é utilizar _underscore_ sobre o _camel case_:

`requisitarUmaMensagemComRepositorioVazio` para `requisitar_uma_mensagem_com_repositorio_vazio`

### Feedbacks

Os excessos no código de teste \(padrões de _feedback_\) diz o quanto estável é a unidade de programação:

* exercícios das responsabilidades: baixa coesão;
* dublês das colaboradoras: alto acoplamento; e
* avalição em colaboradoras: encapsulamento.

Complexidade ciclomática: métrica das ramificações existentes em uma unidade de programação, quanto maior o número, mais complexo e díficil de ser testado será o _software_ \(mais informações em [Medindo a complexidade do seu código](http://blog.caelum.com.br/medindo-a-complexidade-do-seu-codigo/ "Medindo a complexidade do seu código")\).

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

## Técnicas

### O que pensar?

* **AAA\[A\]** - organização e formatação dos casos de teste:

  **A**rrange: monta\/organiza o código com todas as entradas e pré-condições necessárias ao teste;

  **A**ct: exercita\/executa o código sobre teste;

  **A**ssert: avalia os resultados obtidos do código com os esperados pelo teste;

  **A**fter: finaliza os recursos utilizados no teste.

* **FIRST** - propriedades de bons testes:

  **F**ast: rápidos em sua execução, assim mais testes serão avaliados;

  **I**solated: isolados dos outros códigos, assim a verificação da falha será óbvia;

  **R**epeatable: possui repetibilidade em qualquer ordem e tempo;

  **S**elf-validating: automação em sua execução e avaliação;

  **T**imely: em momento oportuno, escreva os testes antes do código.

* **R-&gt;BICEP** - questões sobre os testes:

  **R**ight: os resultados estão certos?;

  **B**oundary: as condições limites estão corretas? Essa é verificada através do **CORRECT**;

  **I**nverse: os relacionamentos inversos \(operações inversas\) estão sendo utilizadas?;

  **C**ross-Check: as checagens cruzadas com outros métodos de mesmo significado estão sendo utilizadas?;

  **E**rror Conditions: as condições de erros estão sendo forçadas?;

  **P**erformance: o desempenho está dentro dos limites?.

* **CORRECT** - as condições limites estão:

  **C**onformance: com os valores conforme o formato especificado?

  **O**rdering: com o conjunto de valores em uma ordem determinada?

  **R**ange: com os valores dentro da faixa \(mínimo e máximo\) especificada?

  **R**eference: com alguma referência externa fora do controle do código?

  **E**xistence: com valor existente \(nulo, zero, presente e etc...\)?

  **C**ardinality: com a quantidade de números suficiente? Os casos interessantes são Zero, Um e Muitos através da regra **0-1-n**.

  **T**ime: com as temporizações corretas \(sincronização, tempo, eventos, referência e etc...\)?


## Boas Práticas

* **Identificação**: ver Documentação.

* **Refatoração**: importante até mesmo para o código de teste.

* **Baby Steps**: começando pelo cenário de teste mais simples em pequenos incrementos, assim ganhando confiança e conhecimento do sistema.

* **Test Data Builders**: utilização do padrão de projeto \(GoF\) _Builder_ para o processo de criação dos objetos para os cenários de testes - auxilia no problema de duplicação de código.

* **Adapters**: utilização para testes com métodos estáticos e códigos legados.

* **Test Double**: isolação de funcionalidades com dependência externa, assim avaliando as características de estado e comportamento do objeto:

  * _Dummy_: _em edição_
  * _Fake_: _em edição_
  * _Stubs_: _em edição_
  * _Mocks_: _em edição_
  * _Spy_: _em edição_

* **Infraestrutura**: a camada de infraestrututra \(_DAO_, _Messages_...\) é testada com testes de integração.

* **Execute Around Method**: utilização para testes com avaliação de exceção.


### Test Smell

_em edição_

