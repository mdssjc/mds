# Caixa Branca
Os testes de caixa branca são conhecidos como **testes unitários**, responsáveis por avaliar e auxiliar no desenvolvimento dos cenários de uma unidade de código.

Esta é uma ferramenta essencial no Desenvolvimento Guiado por Testes - *Test Driven Development* (TDD). Em ferramentas de Integração Contínua - *Continuous Integration* (CI) ocorre a execução automática e avaliativa dos testes.

A proposta básica é que cada **Classe de Equivalência** deve possuir um cenário de teste único.

**Ferramentas:**
* assert (avaliação de sanidade em código)
* JUnit (base dos testes)
* Hamcrest (expressividade de código)
* Mockito (dublê de objetos)
* Infinitest (automação da execução dos testes no cliente)

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
