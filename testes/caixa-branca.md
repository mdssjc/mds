# Caixa Branca
A técnica de teste de caixa branca (*white-box testing*) tem como objetivo avaliar a estrutura interna dos elementos de programação *(técnica estrutural)* durante a etapa de Codificação nas fases de **testes unitários** (*unit testing*) - responsáveis por auxiliar e avaliar no desenvolvimento dos cenários de uma unidade de código (estrutura interna do programa) e/ou **testes de integração ou componentes** (*integration testing or component testing*) - responsáveis por avaliar a comunicação entre objetos e recursos.

A metodogia de Desenvolvimento Guiado por Testes - *Test Driven Development* (TDD) é a utilizada para a etapa de Codificação, na qual os testes são implementados incrementalmente antes do código de produção sempre evoluindo através de refatoração. A implementação do código de produção deve ser o suficiente para os testes resultarem em exito, pois assim protege o código de previsão de funcionalidades e condições. A ferramentas de Integração Contínua - *Continuous Integration* (CI) auxilia na execução automática e avaliativa dos testes.

**Importante o cuidado** para não violar o Princípio da Responsabilidade Única - *Single Responsibility Principle* (SRP) durante a implementação do código sobre teste, pois deve-se testar apenas as funcionalidades expostas (*Tell, Don't Ask*), a proposta básica é que cada **Classe de Equivalência** deve possuir um cenário de teste único e suficiente, ou seja, a inclusão de pequenos incrementos entre testes conforme suas condições limites.

**Elementos de teste:**
* **Java**: Classes;
* **Lisp**: Funções, Comandos e Macros; e
* **C**: Funções.

**Fases do teste:**
*(setup, exercise, verify, teardown) -> em edição*

As [ferramentas](ferramentas.md) mais utilizadas são:
* assert
* JUnit
* Hamcrest
* Mockito

---

## Documentação
Os testes formam a documentação viva do código, logo seus nomes (identificadores) serem pensadas em nível sintático e semântico são de extrema importância, tais como:

* **action**: usa uma ação do cenário de teste, ex: *adicionaUmUsuario*.

* **given-when-then**: relaciona o contexto, ação e resultado, ex: *dadoXQuandoAcontecerYEntaoFacaZ*.

---

## Técnicas
### O que pensar?
* **AAA[A]** - organização e formatação dos testes:

  **A**rrange: monta/organiza o cenário do código com todas as entradas e pré-condições necessárias ao teste;

  **A**ct: exercita/executa o código sobre teste;

  **A**ssert: avalia os resultados obtidos do código com os esperados pelo teste;

  **A**fter: finaliza os recursos utilizados no teste.

* **FIRST** - propriedades de bons testes:

  **F**ast: rápidos em sua execução, assim mais testes serão avaliados;

  **I**solated: isolados dos outros códigos, assim a verificação da falha será óbvia;

  **R**epeatable: possui repetibilidade em qualquer ordem e tempo;

  **S**elf-validating: automação em sua execução e avaliação;

  **T**imely: em momento oportuno, escreva os testes antes do código.

* **R->BICEP** - questões sobre os testes:

  **R**ight: os resultados estão certos?;
  
  **B**oundary: as condições limites estão corretas? Essa é verificada através do **CORRECT**;
  
  **I**nverse: os relacionamentos inversos (operações inversas) estão sendo utilizadas?;
  
  **C**ross-Check: as checagens cruzadas com outros métodos de mesmo significado estão sendo utilizadas?;
  
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

---

## Usos
* **TDD**: empregra os testes como a *principal ferramenta de codificação*, antes mesmo do código de produção, através do seu ciclo:
  
  **Red**: o teste representa cada requisito;

  **Green**: o teste guia a implementação do código; e

  **Refactor**: os testes mantém a integridade do código.
  
* **CI**: *em edição*

* **Testes de Regressão**: *em edição*

---

## Boas Práticas
* **Identificação:** utilização do nome da classe seguido por Test.

* **Test Data Builders:** utilização do padrão de projeto Builder para construção dos objetos para cenário de testes.

* **Adapters:** utilização para testes com métodos estáticos.

* **Mock Objects:** isolação de funcionalidades com dependência externa.

* **Baby Steps:** incrementos em pequenos passos, assim ganhando confiança.

* **Verificar DAO**: *em edição*.

---

## Test Smell
*em edição*