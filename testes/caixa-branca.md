# Caixa Branca
A técnica de teste de caixa branca (*white-box testing*) tem como objetivo avaliar a estrutura interna dos elementos de programação *(técnica estrutural)* durante a etapa de Codificação nas fases de **testes unitários** (*unit testing*) - responsáveis por auxiliar e avaliar no desenvolvimento dos cenários de uma unidade de código (estrutura interna do programa) e/ou **testes de integração ou componentes** (*integration testing or component testing*) - responsáveis por avaliar a comunicação entre objetos e recursos.

Na etapa de Codificação, os testes de caixa branca auxília em:
* **Desenvolvimento Guiado por Testes** - *Test Driven Development* (TDD): empregra os testes como a *principal ferramenta de codificação*, antes mesmo do código de produção, através do seu ciclo:
  * Red: o teste representa cada incremento do requisito;
  * Green: o teste guia a implementação do código; e
  * Refactor: os testes mantém a integridade do código.
* **Integração Contínua** - *Continuous Integration* (CI): auxilia na execução automática e avaliativa dos testes; e
* **Testes de Regressão**: *em edição*.

**Importante o cuidado** para não violar o Princípio da Responsabilidade Única - *Single Responsibility Principle* (SRP) durante a implementação do código sobre teste, pois deve-se testar apenas as funcionalidades expostas (*Tell, Don't Ask*), a proposta básica é que cada **Classe de Equivalência** deve possuir um cenário de teste único e suficiente, ou seja, a inclusão de pequenos incrementos entre testes conforme suas condições limites.

As tecnologias de desenvolvimento possuem elementos mínimos para testes, sendo:
* **Java**: Classes;
* **Lisp**: Funções, Comandos e Macros; e
* **C**: Funções.

Os excessos no código de teste:
* exercícios: baixa coesão;
* dublês: alto acoplamento.

As [ferramentas](ferramentas.md) mais utilizadas são:
* assert
* JUnit
* Hamcrest
* Mockito

---

## Documentação
Os testes formam a documentação viva do código, em que são de extrema importância seus identificadores (nomes dos testes) serem pensadas em nível sintático (relação entre os termos) e semântico (sentido de ideias) com o que será testado, tais como:

* **action**: usa uma ação do cenário de teste, ex: *adicionaUmUsuario*.

* **given-when-then**: relaciona o contexto, ação e resultado, ex: *dadoXQuandoAcontecerYEntaoFacaZ*.

Os identificadores tendem a ficarem longo, assim dificultando em sua leitura - uma dica é utilizar *underscore* sobre o *camel case*:

```requisitarUmaMensagemComRepositorioVazio``` para ```requisitar_uma_mensagem_com_repositorio_vazio```

### Casos de Testes
Os seguintes identificadores são utilizados para os casos de testes:

**NameTest**: testes unitário;

**NameIntegrationTest**: testes de integração; e

**NameSystemTest**: testes de sistema (ver [Caixa Preta](caixa_preta.md)).

---

## Fases do Teste
**Fases do teste:**
*(setup, exercise, verify, teardown) -> em edição*

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

## Boas Práticas
~~* **Identificação**: utilização do nome da classe seguido por Test.~~

* **Test Data Builders**: utilização do padrão de projeto Builder para o processo de criação dos objetos para os cenários de testes - auxilia no problema de duplicação de código.

* **Adapters**: utilização para testes com métodos estáticos.

* **Mock Objects**: isolação de funcionalidades com dependência externa.

* **Baby Steps**: incrementos em pequenos passos, assim ganhando confiança.

* **Verificar DAO**: *em edição*.

* **Execute Around Method**: *em edição*.

---

## Test Smell
*em edição*