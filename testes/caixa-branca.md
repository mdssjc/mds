# Caixa Branca
Os testes de caixa branca (*white-box testing*) são conhecidos como **testes unitários**, responsáveis por auxiliar e avaliar no desenvolvimento dos cenários de uma unidade de código (estrutura interna do programa). **Importante o cuidado** para não violar o Princípio da Responsabilidade Única - *Single Responsibility Principle* (SRP) durante a implementação do código sobre teste, pois deve-se testar apenas as funcionalidades expostas (*Tell, Don't Ask*). Esses testes são tratados como a documentação do código, assim deve-se sua identificação serem pensadas em nível sintático e semântico, as próprias ferramentas de testes incentivam essa técnica como por exemplo o JUnit e Hamcrest.

Esta é uma ferramenta essencial no Desenvolvimento Guiado por Testes - *Test Driven Development* (TDD). Em ferramentas de Integração Contínua - *Continuous Integration* (CI) ocorre a execução automática e avaliativa dos testes.

A proposta básica é que cada **Classe de Equivalência** deve possuir um cenário de teste único.

**Ferramentas:**

* assert (avaliação de sanidade em código)
* JUnit (base dos testes)
* Hamcrest (expressividade na avaliação do código)
* Mockito (dublê de objetos)
* Infinitest (automação da execução dos testes no cliente)

**Documentação:**

Os testes formam a documentação do código, logo seus nomes são de extrama importância, como:

* **action**: usa uma ação do cenário de teste, ex: *adicionaUmUsuario*.

* **given-when-then**: relaciona o contexto, ação e resultado, ex: *dadoXQuandoAcontecerYEntaoFacaZ*.

**Técnicas:**

* **AAA[A]**

  **A**rrange: montar/organizar o cenário do código;

  **A**ct: exercitar/executar o código;

  **A**ssert: avaliar os resultados do código;

  **A**fter: finalizar recursos utilizados no teste.

* **FIRST**

*em edição*

* **B->RIGHT**

*em edição*
 
* **CORRECT**

*em edição*

* **TDD**

  **Red**: *em edição*

  **Green**: *em edição*

  **Refactor**: *em edição*

**Boas Práticas:**

* **Identificação:** utilização do nome da classe seguido por Test.

* **Test Data Builders:** utilização do padrão de projeto Builder para construção dos objetos para cenário de testes.

* **Adapters:** utilização para testes com métodos estáticos.

* **Mock Objects:** isolação de funcionalidades com dependência externa.

* **Baby Steps:** incrementos em pequenos passos, assim ganhando confiança.